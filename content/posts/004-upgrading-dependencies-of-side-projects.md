---
title: "working title"
date: 2025-03-31T10:00:00+01:00
tags:
  - sideprojects
  - dependencies
comments: true
---

Have you ever had a side project that you havent't been working on for a long time? Well for me there is a project I started in 2021 mainly to do my homework at school a little faster. It is a webapp that was able to solve some simple math problems. A few days ago I decided to no longer update the dependencies of this project. It was a hard decision for me personally. I want to share my experience with this with you. Maybe it can be helpful for you if you are facing an similar decision to follow my train of thought.

## How was the codebase? (working title)

Well to say it short: The codebase is from todays perspective a total mess. 

The project was created during my early days as a software engineer. I wanted to learn a new framework and devided to go with svelte kit which was in the open beta at that time. So I decided to give it a shot. To be fair it was a pretty great experience working with it. But after a few months I stopped working on it, because I stopped doing my math homework lol. 
Therefore, there was no real progress over the past years within this project. It is all old beta framework code. Pretty bad code to be fair, because I was unexperienced at that time.

Doing the required changes to bump up the project to the latest dependencies would take a lot of effort. First of all I would have to resolve the dependency mess. There are some old npm dependencies that are nowadays no longer supported or no longer needed, because svelte kit now does it itself. 

After cleaning up the dependencies I will still have to migrate all the code. Modern best practises of how to write good svelte kit code. Furthermore, I am not really sure how some things work today in svelte kit so I would have to do also some research on those topics to fully understand all these new stuff.

## What were the influencing factors? (working title)

There were some factors influencing my decisions on this topic.

First of all there is the effort that is required to do the migration to the latest version of svelte kit. As I already mentioned it is quite complex and will take an vast amount of time. Due to some big changes in how svelte kit works over the past years I would have to nearly rewrite all of the code. Sure a lot of logic can be copied but nevertheless it would be pretty complex. Furthermore, the process of finding all the right dependency replacements for existing and non-existing functionality in the framework itself could also take some time. Svelte CLI is now replaced by vite for example. Therefore, I will need to find replacements for static export and some other topics. 

Furthermore, there are no real security risks of not upgrading the dependencies. The application is just a simple webapp. It runs exclusively in the browser. It does not rely on external services nor any backend. Therefore, I can say with confidence that not upgrading the dependencies does not cause any security issues. In addition to that there are no real users of the project. So I would only do this migration for myself. Not for a large userbase.

On the other hand I want to learn all the new techniques and tricks that svelte kit has to offer today. But I also feel somehow triggered of the fact that I do not upgraded my dependencies on purpose. It would cause an emotional conflict in myself, because I have pretty high standards to myself. Sure, I do not do the best work and I am by far not the best developer, but I want to regulary challenge myself to improve. And not doing these migrations on purpose feels like escaping these challenges, which triggers me.

Finally, there is a more emotional factor: I actually like the codebase. The codebase is like a memory to me. It reminds me of the 2021 version of me working on this project. This legacy code I wrote almost 4 years ago is pretty bad, but it is somehow also a beauty to me. It is an emotional memory and erasing it by refactoring the code would also raise an conflict inside me. But to be fair, this argument is less weighted than the other ones. 

## What was my final decision and why?

- The total required effort, the low amount of users and the low security risk were factors that heavily stated that I should not upgrade the dependencies.
- But the personal influence factors like learning new svelte (I can do this also with a new project) and the trigering factor of an project of mine not being upgraded on purpose also had an heavy impact.
- Finally, yes I somehow liked the code I was watching at and working with.
- So I decided to act rationally and not emotionally and dropped dependency upgrades for this project.

## What can you learn from all this?

- These personal decisions are very hard for everyone.
- In the end you have to evaluate all the factors for yourself. If the project has a high emotional value for you, keep working on it
- But if you can't find a proper decision you will need to decide damn rationally. Sure, this might feel bad in the first place. But in the end it is the right decision. Like in my case. I really loved this project, because it was one of my first web projects I worked on longer than 2 months. But even if this project had such an high emotional value to me, it was right to not upgrade the dependencies anymore. It wouldn't be worth the effort. And I still can work on it. But only with beta status dependencies. And I really love the experience with it.
- So in the end the rational decision might be also the decision that is emotionally the best for you. It's a win for both.