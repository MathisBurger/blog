---
title: "When to Stop Updating a Side Project — and Why I Did"
date: 2025-04-01T1:00:00+01:00
tags:
  - sideprojects
  - dependencies
comments: true
---

Have you ever had a side project that you haven't worked on in a long time? For me, there’s a project I started in 2021, originally to help me complete my school homework a bit faster. It’s a web app capable of solving simple math problems.

A few days ago, I made the difficult decision to stop updating its dependencies. Letting go of this project was not easy for me. That’s why I want to share my experience with you—perhaps my thought process will be helpful if you ever find yourself facing a similar decision.

## The projects starting point

To put it simply: from today’s perspective, the codebase is a complete mess.

I started this project in my early days as a software engineer. I wanted to learn a new framework and decided to go with SvelteKit, which was still in open beta at the time. So, I gave it a shot. To be fair, working with it was a great experience. But after a few months, I stopped working on the project—mainly because I stopped doing my math homework, lol.

As a result, there has been no real progress over the past few years. The entire project is based on outdated beta framework code. And to be honest, the code itself isn’t great—it reflects my lack of experience at the time.

Updating the project to the latest dependencies would require a significant amount of effort. First, I’d need to untangle the dependency mess. Some of the old npm dependencies are no longer supported or even necessary, as SvelteKit now provides built-in solutions for them.

Even after cleaning up the dependencies, I’d still have to refactor and migrate all the code to follow modern best practices for SvelteKit. On top of that, I’m not entirely sure how certain things work in SvelteKit today, so I’d need to do some research to fully understand all the new changes.

## Influencing factors

Several factors influenced my decision on this topic.

First and foremost, there’s the effort required to migrate the project to the latest version of SvelteKit. As I’ve already mentioned, the process is quite complex and would demand a vast amount of time. Due to significant changes in how SvelteKit works, I would need to rewrite almost all of the code. While much of the logic could be reused, the migration would still be challenging. Additionally, finding suitable replacements for deprecated dependencies and framework functionality could be time-consuming. For example, Svelte CLI has been replaced by Vite, meaning I’d need to find new solutions for static exports and other features.

Another key factor is that there are no real security risks in not upgrading the dependencies. The application is a simple web app that runs entirely in the browser. It does not rely on external services or a backend, so I can confidently say that leaving the dependencies as they are does not introduce any security concerns. Moreover, the project has no real users—this migration would be purely for myself, not for a larger user base.

On the other hand, I do want to learn about the new techniques and improvements in SvelteKit. At the same time, deliberately choosing not to upgrade the dependencies creates an internal conflict for me. I hold myself to high standards—not because I think I’m the best developer, but because I want to continuously challenge myself and improve. Avoiding this migration on purpose feels like avoiding a challenge, which bothers me.

Lastly, there’s an emotional aspect to consider: I actually like this codebase. It serves as a memory of my 2021 self working on this project. Even though the code is objectively bad, I still find it somewhat beautiful. Refactoring it would feel like erasing a piece of that memory, which creates another internal conflict. That said, this emotional argument carries less weight compared to the practical considerations.

## Final decision

Reaching a final decision was difficult. The significant effort required, the lack of users, and the minimal security risk were key factors in my decision-making process. I don’t have much free time to dedicate to personal projects, and upgrading the dependencies would consume a large portion of it—something I wasn’t willing to sacrifice.

Learning modern SvelteKit could just as easily be done with a new project. However, the thought of avoiding a challenge still weighed on me. And then there was the emotional aspect—I genuinely like my legacy code because it reminds me of the "good old days".

In the end, I had to make a choice. I decided to act rationally rather than emotionally and ultimately chose to stop upgrading the dependencies of this project.

## What can you learn from all this?

Personal decisions like this are difficult for everyone. That’s why I believe you might gain something from my thought process.

In the end, you have to make your own decisions. Simply copying mine would be the worst possible approach to tackling your own challenges. When facing a similar dilemma, you should certainly consider the emotional value of your project. However, it’s equally important to think rationally about all the influencing factors. Acting rationally while setting emotions aside can be difficult at first, but trust me—it will ultimately lead to the right decision.

Of course, emotions matter. And in project management, they are crucial when working with team members. But when it comes to the hard facts of a project itself (rather than the human component), decisions should be made rationally.

Take my case, for example. I loved this project—it was one of my first web development projects, and I worked on it for over two months. It had significant emotional value to me. Yet, deciding not to upgrade the dependencies was still the right choice. The effort simply wouldn’t have been worth it. I can still work on the project, but only with its outdated beta framework.

As I said, emotions are important, but so are the hard facts. When collaborating with others, their emotions and perspectives should be a priority. But when it comes to making technical decisions about the project itself, a fully rational approach is the best way to achieve the best outcome. In the end, acting rationally benefits everyone involved—it’s a win for all.