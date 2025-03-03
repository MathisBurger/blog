---
title: "Your learning sideprojects code can be shitty"
date: 2025-03-02T19:08:53+01:00
tags:
  - sideprojects
  - code-quality
  - learning
---
In the past few days, I have been working on a side project that uses PHP and [Laravel](https://laravel.com/). I should mention that I had never used Laravel before in my life. My professional experience has primarily been with other PHP frameworks, like [Symfony](https://symfony.com/), and I thought: Why not try something new?

I believe many people feel the same way. They want to explore something they’ve never worked with before. This is the essence of lifelong learning, especially in software engineering. In this field, you’re always learning new things, and that’s one of the reasons I love it so much.


## Sideprojects for learning?

Well, you know, I'm more of a practical person. When I want to learn something new, I can’t just go through examples or walk through all the playgrounds the language or framework might offer. The approach that works best for me is to actually build a project with the framework or language. I’ve spoken to many people, and most of them agree with this. Learning in a practical way through a project is much more enjoyable, and you can see your actual progress.

I have a fairly long list of side project ideas I want to develop someday. For learning Laravel, I simply picked one of those ideas. In this case, it was a simple web application where my friends and I could create fun bets and place our wagers on them. Pretty simple, not overly complex. I also added some additional requirements to explore the capabilities of the framework and see how easy and pleasant it is to develop with. Examples include localization and notifications within the web app.

In my opinion, this is a great deal. You’re working on some of your side project ideas while simultaneously learning something new. It seems like a win-win. Well, it's not always that easy...


## The learning curve

When you’re learning something new, there are often patterns or best practices you haven’t encountered yet. You might have discovered them if you had first read the documentation. But let’s be honest: While most people do read the docs, they might forget certain things when they’re actually developing. You can’t know everything right away. Knowledge comes from experience and repetition. It comes from failing and spending hours debugging a simple problem, rather than solely preparing by reading the documentation.

However, as you learn the framework or language, you get better at it. After a few hours or days, you start to pick up the basic patterns. In the case of Laravel, for example, you learn how the ORM works and how to handle database connections. You learn how to implement controllers and use Blade. You also discover best practices for organizing the file structure of your components.

How easily you can learn something new often depends on what you’ve already learned. It might seem a bit confusing, but let me explain what I mean: Imagine someone who has spent their entire career working in the object-oriented programming (OOP) world of Java. This person knows everything about object-oriented programming, and these concepts are deeply ingrained in their mind. Now, imagine this person learning React. While they might be comfortable with class components, they could struggle with things like hooks, functional components, and other non-OOP concepts. On the other hand, this person might find Angular easier to learn because its patterns are more similar to Java’s.

## Refactoring hell

After you've learned a lot about this new technology, you might look at your project and think, "How did I build this?" And honestly, that’s completely normal. When you started this project, you had no idea how things worked. You might have used a file structure that isn’t considered best practice, or perhaps you put logic that belongs in a repository directly inside your controller.

At this point, you have two options: leave it as it is or start refactoring everything. Depending on the size of your project, this could take a significant amount of time. You might be thinking it would have been better to read the documentation from the start, but I actually don’t agree with that. Think about what would have happened if you had just read the documentation: Sure, you might have followed some best practices, but you wouldn't have learned nearly as much.

When I think about my experience with Laravel, I remember long debugging sessions where I tried to figure out how things worked. I dug deep into the framework's internals to understand how it operates under the hood, rather than just learning the basics needed to get the job done. Sure, the first approach would have been easier, but because I took the time to understand the framework better, I now know how to solve problems when they arise. So, even if you now find yourself needing to refactor your entire side project, you've gained some serious skills. Sure, choosing the quickest way to get things done isn’t inherently bad, but in the long run, the more challenging approach might actually help you work more efficiently.

Of course, you might not have approached the problem the best way when you tried to fix it on your own. There could have been an abstraction in the language or framework that would have made things easier. You could have used it right away, but now you have a deeper understanding of your technology and how it works. That’s still a win.

## Your sideproject is no system critical infrastructure

But the question still remains: Should you refactor your entire codebase or not? I would say it depends. It’s a pretty personal decision. Personally, I would always try to refactor it. If the result isn’t worth the effort, you can limit your refactoring to the basics. But what you should keep in mind is that your side project is not critical infrastructure.

Let’s be honest—most of us start a side project without much planning. We get an idea and start coding right away. There’s no use-case analysis, no UML class diagrams. Maybe some component designs, but even that’s rare for side projects (at least for me). The main purpose of side projects is to have fun. We’re not building the backend of a billion-dollar enterprise here. These projects are not meant to be that formal. Side projects should give developers the freedom to do whatever they want, without any restrictions on component design or even best practices. The goal is fun and learning.

So please, stop overengineering your side projects. If you’re realistic, the primary users of such a project will likely be you and your friends. There’s no need to consider a microservice architecture just to scale to a million users at once. But if you enjoy thinking about those problems, feel free to dive into them.

## But should I read the docs?

Earlier in this article, I mentioned that you shouldn't read the documentation. That’s not entirely accurate. Of course, you should definitely read the docs to gain a basic understanding of how everything works. What I meant was that you don’t need to read the entire documentation in detail before starting your project.

Over the years, I’ve developed a personal approach to using documentation for new projects. First, I think about what I’ll need initially. In the case of my side project, it was routing, basic REST APIs, and database interaction. So, I sat down and skimmed through the docs to get an idea of how things work. Then, I started working on my project. When I run into a problem, I first try to solve it on my own. Through this process, I learn how the framework works. For example, if I need to retrieve a search query parameter from the HTTP request URI, I don’t immediately look up the documentation. Instead, I check out the Request object that's passed to my controller and explore its API to see if it provides a solution. This way, I not only learn how to retrieve a search parameter from the URI, but also how the API works in general, which prepares me for future problems.

This might seem like the harder and more time-consuming approach at first, but it will pay off in the long run. There’s always the shortcut of reading the documentation, browsing Stack Overflow, or nowadays using ChatGPT or another chatbot to solve your problems. But throughout your career, you’ll also work with technologies that are less well-known or not as thoroughly documented. In those cases, you’ll need to understand how the framework or language works internally to solve problems effectively.

Let me give you an example: In my professional career, I’ve been working a lot with the PHP framework Symfony. It’s well-documented and relatively easy to start with, but it also has a steep learning curve because it simplifies many things. However, like any other framework, it can become quite complex. In one project, I had to work with a library that instantiated an admin dashboard. I wanted to override some form submission behavior, but the problem was that the Symfony docs didn’t cover this scenario, because the admin dashboard library added an extra abstraction layer on top of the Symfony API. Stack Overflow wasn’t much help either, since this wasn’t a common use case for overriding form submission behavior. To solve the problem, I had to understand how the Symfony API worked internally in order to hook into the form submission process and make the required changes. Without learning Symfony the hard way, I would never have been able to do that.


## Conslusion

So, what can you learn from all this? The main focus of side projects is to have fun. You shouldn’t restrict yourself with unnecessary limitations. They’re perfect for learning something new because they aren’t major commitments, giving you more room to experiment, make mistakes, and learn from them. And yes, your code might end up looking pretty bad, and you’ll probably need to refactor it. But take a look at your first projects with the technology you’re currently most proficient in—weren’t they pretty bad, too? You always improve. And if you want to, you can refactor your project later with the experience and expertise you’ve gained so far.

The second takeaway is that you should definitely read the docs. But you should also challenge yourself. Don’t make it too easy. If learning a new technology feels easy, you probably haven’t learned much. Sure, things might be similar, but if there’s no difference, they’re essentially the same. So, try solving a problem without immediately checking the docs or asking a chatbot. Instead, figure out how things work and how you can use them. This approach leads to more expertise than just reading the docs because you’ll truly understand the technology, how it works, and how to use it. You won’t just know about it—you’ll have hands-on experience.

So, never stop learning and never stop challenging yourself, because doing so would mean you’re not learning anything. Failing makes you a better programmer than just reading about it.

Finally, a motivational quote for you:

*Just let them know that we have a finite amount of time on this planet and you can be viciously mediocre or you can get the fuck after it.* ~ idk who said that
