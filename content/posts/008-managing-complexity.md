---
title: "Why managing complexity in software engineering is the key to everything"
date: 2026-08-07T1:00:00+01:00
tags:
  - complexity 
  - software
comments: true
---

*A quick note before you read on: I started writing this post a while ago and never quite finished it. I'm publishing it now as it was, rough edges and all, because I still think the core ideas hold up. That said, I've learned a lot more about this topic since I first wrote these paragraphs, and I'm sure I'll end up writing a more thorough, more nuanced version of this post in a few years, once I've spent more time actually living with the consequences of the ideas below and doing some more scientific research.*

Everytime I faced a problem in the software engineering process, it was somewhat related to poor complexity management.
You might not think it is related to complexity issues, but at some point it is.

## What is complexity exactly?

Complexity is a multi-faceted term. I won't use some encyclopedia description made up of hard to understand phrases in order to explain it. Let me give you some probably relatable examples instead.

Everytime you wonder why the code looks like a mess, it's because you did not manage to gauge the complexity of the function beforehand and ended up building it without thinking about how to split it up or write it in a more readable way.
If you've read the Clean Code book you might know that you can write a whole philosophy on the readability of code. Complexity is exactly that. Complex code is harder to read, and therefore also harder to understand. You can reduce complexity by splitting up your functions into smaller functions that each do exactly one single thing. That reduces the complexity of each individual function to a minimum and makes the overall complexity more manageable and easier to oversee.

This also relates to the number of parameters you can pass to a function. The more parameters, or the more complex those parameters are, the more unpredictable the actual outcome of the function becomes.
Let's compare those two functions:

```rust
// Function one
fn do_something(a: u32) -> u32

// Function two
fn do_something_else(a: u32, b: HashSet<Vec<HashMap<String, String>>>, c: bool) -> u32
```

As you can see, the second function is a lot more complex. We have three parameters, of which the second one is a very complex datatype. Testing this is a nightmare. You won't even get close to an acceptable test coverage. And even if you get there, how do you ensure the thing actually works as expected?

Ensuring the integrity of the whole software gets even harder when a function requires interaction with other classes or services. It's pretty straightforward to unit test a single class, or even multiple classes independently.
It starts to get really tricky when you have to integrate different components together.

## Where is complexity management most important?

Complexity management matters most when you have multiple services or components in a system that are loosely coupled. You often don't know which service will communicate with which other service. It's a nightmare to manage, debug and prevent.

Let me give you an extreme example: car software.

Modern cars are more like a driving smartphone than our classic understanding of a vehicle. And they have one specialty that is a nightmare in terms of complexity management: they are highly configurable. I bet everyone has, at some point, opened the website of a premium car manufacturer like Porsche, Audi, BMW or Mercedes and configured their dream car. But have you ever thought about what this configurability means for complexity?

Just imagine how many different configuration options for seats there are: normal or sport seats, heating or no heating, cooling or no cooling, massage or no massage, leather or fabric. All of those are almost freely configurable. That's 2^5 = 32 different seats! And almost all of those options have an effect on the underlying software. Now imagine all the other options you can pick during the configuration process.

Without proper complexity management, it's impossible to ensure the car works as expected at all. Of course this is an extreme example, but there are plenty of other applications that handle very loosely coupled use cases and can lead to unwanted side effects in the same way.

Let me give you another example, a more regular one this time. Microservices are a modern trend. Everyone implements applications using them, and they are often developed within an event driven architecture.
This means every service does not call any other service directly, but goes through a message broker instead. So we actually don't always know where a message is being processed and where it isn't. Debugging this is a nightmare, because you can run into side effects and bugs that are caused purely by the sheer complexity of those architectures. This is exactly why companies like Celonis exist. Their whole business is finding out what actually happened inside those highly loosely coupled, distributed architectures.
If you haven't done proper complexity management, I wish you the best of luck being on call and trying to find the cause of the random bug that just took your production environment down.

Log monitoring might help you find the bug, but it does not solve the root cause: complexity. If your system is too complex for you to know what happened, you must either ensure that certain things can only happen under certain conditions (and document those conditions properly, and keep that documentation up to date), or you have to rebuild parts of the system from the ground up so that you can actually handle the complexity of the overall application.

## How can I manage complexity then?

I already talked a little about how to manage complexity, but let me dig a bit deeper now.

One of the simplest tools you have is the Law of Demeter, sometimes described as "only talk to your immediate friends." Instead of reaching through an object to grab something from an object it holds, and then reaching further into that, you ask the object directly for what you need. Every extra hop you allow through your codebase is another hidden dependency between parts of your system that were never supposed to know about each other. The Law of Demeter forces you to keep those chains short, which keeps the blast radius of any change small and predictable.

Closely related is the difference between abstraction and indirection, two things people tend to confuse. Abstraction hides complexity behind a simpler interface, so the caller genuinely has less to think about. Indirection just moves the complexity somewhere else without actually reducing it, and often adds a layer you now have to jump through to understand what's really going on. Good complexity management is mostly about honest abstraction. Bad complexity management is often indirection wearing an abstraction's clothes: an extra layer, an extra interface, an extra factory, that makes the code look cleaner while making it strictly harder to reason about.

Pure functions help here too. A function that only depends on its inputs and only produces an output, without touching global state or reaching out to some shared mutable variable somewhere else, is trivial to test and trivial to reason about. You can look at its signature and know exactly what it can and cannot do. The moment a function starts depending on the outside world, whether that's a global, a database, or some hidden singleton, you lose that guarantee, and the number of scenarios you have to think through to trust the function explodes.

At the architectural level, Bounded Contexts, a concept from Domain-Driven Design, are one of the most effective tools for taming complexity in larger systems. Instead of trying to build one giant, shared model of your entire domain that every team and every service has to agree on, you draw explicit boundaries around areas of the business where a model, its language and its rules stay consistent. Outside that boundary, the same word can mean something different, and that's fine, because the boundary itself is where translation happens. This keeps individual contexts small enough to actually understand, instead of forcing everyone to hold the entire system in their head at once.

CQRS, Command Query Responsibility Segregation, tackles a different kind of complexity: the complexity that comes from trying to make a single model serve both reads and writes equally well. By splitting the write side from the read side, you can let each of them evolve independently, optimize them separately, and avoid the situation where every feature added to one side quietly makes the other side more complicated too.

Finally, for complex distributed systems, it can be worth employing formal analysis using feature models to find dependencies and analyse the tree of connections between components. Feature models let you make the variability of your system explicit, as a structure you can actually inspect and reason about, instead of something that only lives implicitly in configuration files, environment flags and tribal knowledge. Once that variability is visible, you can start actively reducing it instead of just living with it.

If you ask me, feature models are the most promising tool when you have legacy systems that are just hard to refactor properly or when you are building highly complex distributed systems with shared functionality and a lot of indirect interaction. But as I am still conducting more research into that direction, I haven't fully made up my mind about that
certain technology. Nevertheless, feature models can definitely help to visualize your variability through feature model counting.

## Let's put it all together

None of these tools are a silver bullet on their own, and that's kind of the point. Complexity management isn't a single technique you apply once and then forget about, it's a mindset you carry into every decision you make while building software: how many parameters does this function need, does this class really need to know about that other class, does this boundary actually reflect how the business thinks about this concept, or is it just how the code happened to grow.

The car configurator example and the microservices example both point at the same underlying truth: complexity doesn't announce itself. It creeps in one seemingly reasonable decision at a time, one more parameter, one more service, one more shared piece of state, until one day you're on call at 3am trying to figure out why production is down, and the honest answer is that nobody fully understands the system anymore.

The good news is that every tool I've mentioned here, the Law of Demeter, pure functions, bounded contexts, CQRS, feature models, exists precisely because other engineers ran into the same wall before you did. You don't have to rediscover all of this the hard way. Start small: keep your functions honest, keep your dependencies short, and draw your boundaries on purpose instead of by accident. Complexity will never fully go away, but it can absolutely be managed, and that, more than any specific pattern, is the actual skill worth building.
