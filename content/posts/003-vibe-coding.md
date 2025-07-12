---
title: "Vibe Coding is shit. Stop it"
date: 2025-07-12T1:00:00+01:00
tags:
  - AI
  - vibe coding
comments: true
---

Vibe coding seems to be everywhere these days. Social media is flooded with stories of people building SaaS products at record speed using so-called vibe coding techniques. These posts often come with bold claims, not just about productivity but also about the future of our profession. The underlying message is clear: software engineers will soon be obsolete, replaced by AI and no-code tools.

I strongly disagree with this narrative and frankly, I find the whole trend deeply frustrating. Most of these vibe-coded apps are not only rushed but also poorly architected and alarmingly insecure. What is being celebrated as innovation often lacks the fundamentals of sustainable and responsible software development.

## Vibe Coding is not only using AI

As far as I know, there is no clear or widely accepted definition of vibe coding. So before I continue, let me explain what I personally mean by it.

To me, vibe coding is not simply about using AI to assist in software development. That distinction is important. When you use AI as a tool, for example to generate boilerplate code, refactor functions, or get unstuck, you typically have a solid understanding of software development fundamentals. You know how to design architecture, apply appropriate software design patterns, and critically assess the code you write, including code suggested by AI. You are able to spot mistakes and poor practices because you understand the broader context.

Vibe coding is something different. It is more abstract and, frankly, more careless. In vibe coding, the AI effectively becomes the architect. It chooses the patterns, structures the code, and makes key decisions while the developer blindly follows along. There is little concern for how things are implemented, as long as they appear to work and the application looks functional on the surface.

This, in my view, is exactly how many of the new, self-proclaimed “cool” SaaS builders operate online. It is thirty percent coding and seventy percent tweeting about how revolutionary their AI-written note-taking app is, often without any understanding of what is actually going on under the hood.

## Why is vibe coding bad?

By now, you can probably already imagine why vibe coding is such a bad idea.

You’re essentially pushing code to production without any real verification. And how could you verify anything when you don’t actually understand what the code is doing in the first place? Without a solid grasp of software development, you’re left blindly trusting that whatever the AI generates is correct, secure, and maintainable, which is wishful thinking at best.

It’s like deploying an application and simply hoping that it’s not vulnerable, that everything magically works as intended, and that no edge cases will ever break it. Spoiler: they will. 

<img src="/003-ai-doctor.jpg" width="50%" />

*Unfortunately, I no longer remember where I originally found this image. If you happen to recognize it, please let me know so I can give proper credit.*

I believe this image perfectly captures why vibe coding is such a huge problem.

AI confidently provides output that looks correct until you ask the right question. But to ask the right question, you need to understand what the code is actually doing. And that is exactly the issue: many people do not.

We have all seen examples of developers accidentally committing API keys to public GitHub repositories or deploying highly insecure applications simply because they lacked the knowledge to question the AI’s output. This is not a rare mistake; it is the consequence of not knowing enough to validate or challenge what the machine suggests. That is why vibe coding is not just misguided, it is dangerous. In the past, the barrier to writing code was that you had to know how to do it. Now, with vibe coding, you can build and deploy something without truly understanding software development. That might sound empowering at first, but on closer inspection, it introduces serious risks.

Software engineers are engineers. Would you feel safe driving a car that was vibe engineered by someone with no training in mechanical engineering? Would you take medication developed by a vibe pharmacist? Most likely not. Sure, software might seem more harmless, but it can still be critically vulnerable. Storing passwords in plain text, skipping hashing and salting, means one data breach and your password, which you probably use for multiple accounts, is out in the wild. Even if it is just your email address, that is enough for phishing, spam, and identity fraud.

When I use an application, I want it to be secure and not accidentally secure. Most of all, I want it to work as designed, not as vaguely intended by an AI. That is a big difference. Maybe it is just me, but I am genuinely worried about the direction this is heading. Do not get me wrong, AI is an incredible leap forward for developer productivity. But replacing developers altogether might turn out to be a massive mistake.


## The limitations of AI

AI is undeniably good at certain things, especially when it comes to writing boilerplate code or suggesting best practices. For common, well-documented problems, it often delivers solid results. Tasks that have been solved countless times before, AI can handle those reasonably well.

But the moment your problem becomes even slightly more complex, things start to fall apart. Take this example: writing simple database pagination in Rust using Diesel is no problem for most AI models. However, introduce just one extra trait bound into the mix, and suddenly no model seems to get it right. Despite the fact that the correct solution is relatively straightforward for someone with a bit of Rust experience, the AI fails.

This illustrates a deeper issue. AI is fantastic for repetitive, boring tasks. It can help generate tedious glue code, refactor existing logic, or even provide high-level scaffolding. But it still struggles with semi-complex problem solving, especially in more niche or strongly typed languages like Rust.

That is because today’s most powerful models are still narrow AI. They do not truly understand what they are doing. They cannot generalize, adapt, or reason beyond what they have seen. They are built to mimic, not to think. They rely entirely on patterns and examples found in the training data, code written by humans, often taken from the public internet. And here is the problem: as the internet becomes more and more flooded with unchecked AI-generated code, the quality of that training data will inevitably decline. This creates a feedback loop that could make future AI models worse at programming, not better.

The real breakthrough would be Artificial General Intelligence, or AGI. That is the holy grail, an AI that can truly reason, learn, and solve problems across domains. But despite billions of dollars in research, AGI remains a very distant and very uncertain goal. It may never be achieved.

So please stop telling developers they are about to be replaced, especially when your entire coding experience consists of launching a painfully insecure and painfully slow SaaS that barely has five users. No, I am not afraid of the future and I am certainly not afraid of losing my job. What I am concerned about is the growing trend of people refusing to think critically. Evolving with technology means understanding it and using it responsibly, not blindly outsourcing your thinking to it.

Will some developer roles disappear? Probably. With AI taking over more repetitive tasks and templated design patterns, the demand for junior developers might shrink. But will software engineers as a whole vanish? That is far from certain, and frankly, I doubt it.


## How to use AI properly

In my opinion, AI is just another tool, a powerful one that can significantly boost developer productivity. But like with any tool, the key is knowing how to use it properly. And the most important rule is to always verify what the AI gives you.

If you do not understand the code, do not use it. Try to understand it first. Treat AI-generated code like you would code from a teammate. Review it thoroughly, test every edge case you can think of, and do not trust it blindly.

Let us take a simple example. Imagine you are building a REST API with basic CRUD operations and your database schema is already defined. That is a task AI can easily handle, saving you maybe 30 minutes of routine work. But once the code is written, your job is not done. You need to ask yourself if authorization is implemented correctly, if the right properties are exposed through the API or worse, if there are any sensitive fields leaking out. Are the database queries efficient? Is caching implemented in a sensible way? Is there proper rate limiting? And are the endpoints named consistently and meaningfully?

Only after checking all of these things and making the necessary improvements is the code truly safe and ready to use.

In fact, this blog post is also partly written with AI. I created the bullet points and structure and the AI helped shape them into coherent text. But I reviewed and validated every section. That is exactly how it should be. AI assists, you remain in control.

When you encounter something new, you can absolutely use AI to support your learning process. But do not start by asking it to write the solution. First, think through the problem yourself. What would be an efficient and clean solution? Only then should you turn to AI, not to write code for you but to provide background information, suggest known algorithms, or point you to RFCs and technical standards that are relevant to your use case.

With that knowledge you are in a much better position to write correct and understandable code and more importantly to reason about it.

It really is that simple.

When learning new things, AI can be a solid partner. It can help prepare study material or generate more advanced questions to test your understanding. It is a great tool for accelerating learning but it should never replace your own thinking.

AI has the potential to boost your productivity beyond what was possible with traditional tools. But it should stay what it is, a tool. If you let AI do all the thinking, your value as a developer drops to zero.

So do not be careless. Do not be passive. Use your brain.

