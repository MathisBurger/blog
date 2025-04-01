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

Getting to the final decision was hard. The total required effort, the low amount of users and the low security risk were factors that heavily influenced my decision making process. I do not have much free time where I can focus on my private projects. So therefore upgrading the dependencies would take a hell of a lot of my freetime, which I didn't really wanted.

Learning modern svelte kit could also be acchieved with a new project. But the triggering factor of escaping to self challenge myself also hit hard. And there is also the factor that I do like my legacy code because it reminds me of the "good old times".

So I had to make a decision. And I decided to act rationally and not emotionally and decided to do not upgrade all the dependencies of my project anymore. 

## What can you learn from all this?

These personal decisions are very hard for everyone out there. Therefore I think that you might can learn something from my personal train of thought on this. 

In the end you will have to do all the decisions on your own. You should not copy my decision one by one. This would be the worst possible approach to tackle your problems. But when you are facing such a problem, sure you should ask yourself how high is the emotional value of this project for you. But you should also think rationally about all the influencing factors. Acting rationally and ignoring emotional factors might be hard in the first place, but trust me, in the end it will be the right decision. Of course, emotions are important. And if you are working in project management, emotions are very important when your talking about the other team members. But when it comes to the hard facts about the project itself (and not the human component of it) you should definetly decide rationally. 

It's like in my case. I really loved the project, because it was one of my first projects in web development I have been working for more than two months on. The project had an pretty high emotional value to me, yes. But it was right to do not upgrade the dependencies anyway. It wouldn't be worth the effort. I can still continue working on the project. But only with the beta status framework. 

As I already said, emotions are important but so are the hard paper facts. When working with other people, their emotions and feelings should have a high value for you. But the decisions on the project itself should be 100% rationally to get the best out of it. Acting rationally is in this case be best thing you can do for all participants of the project. It's a win for all.