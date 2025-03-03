---
title: "Your learning sideprojects code can be shitty"
date: 2025-03-02T19:08:53+01:00
tags:
  - sideprojects
  - code-quality
  - learning
---

In the last days I have been working on an side project which uses PHP and [Laravel](https://laravel.com/). You might have to know, that I have never been using Laravel before in my entire life. I have worked with other PHP frameworks like [Symfony](https://symfony.com/) for my entire professional career and thought: Why not try out something new?

I think many people do feel like this. They want to try something new, they have never been working with. This is how lifelong learning and especially software engineering works. You never stop learning new things in this field which is why I love it so much.


## Sideprojects for learning?

Well you know, I am a more practial person. When I want to learn something new I cannot just do the examples and walkthrough all the playground the language or framework might offer. The approach I learn the most is that I actually do a project with this framework or language. I have spoken to many people and most of them can agree on this. Learning it the practical way through a project is way more fun. You can see your actual progress.

I have a pretty long list of sideproject ideas I want to develop some day. And for learning Laravel I just picked one of the many ideas. In this case it was just a simple web application where my friends and I can create fun bets and place our bets on it. Pretty simple. Not that complex. I also added some requirements to check out the abilities of the framework and how nice and easy things are to develop with it. Some examples for that are localization or notifications in the web app itself. 

In my opinion this is a pretty good deal. You are actually doing some of your side project ideas and at the same time learning something new. Semms like a world without any problems. Well, it is not that easy...


## The learning curve

When you learning something new, there are often some patterns or best practises you do not know yet. You maybe would have known them, if you first have read the docs. But let's be honest: Most people do read the docs, but when actually developing something they might forget things. You cannot know everything. The knowledge comes from experience and repetition. It comes from failing and 10 hours of debugging over a simple problem rather than from preparing by reading the docs. 

But while you are learning the framework or language you are getting better in it. After a few hours or days you get to know the basic patterns. In case of Laravel you learn how the ORM works and how database connections are used. You learn how to implement controllers and how to use Blade. But you also learn about best practises for the file structure of your components. 

How easy you can learn something new always depends on the things you have already learned. Might seem a little confusing, but let me show you what I mean: Imagine a person that is working his whole life in the OOP world of Java. This person knows anything about object-oriented programming and these concepts are depply burned into its mind. Now imagine this person learning React. This person might feel familiar with class components, but when it comes to things like hooks, functional components and other non-OOP stuff, this person might have a hard time learning it. This person might have a more fun time learning angular, because the patterns are more similar to Java.

## Refactoring hell

After you have learnt a lot about this new technology, you might take a look at your project and think: How did I built this piece of shit? And well, this is completely normal. When starting this project you had absolutely no idea how things worked. You might have used a file structure that is not best practise or you might have put logic that belongs into a repository diretly inside your controller. 

Now you have got two options. Keep it like it is or start refactoring everything. Depending on the size of your projet this could take a huge amount of time. At this point you might think it would have been better to read the documentation in the first place, but I actually do not agree with this. Think about what would have happend if you just have read the documentation: Sure, you might have followed some of the best practises. But I would never have learned nearly as much. 

When I think about my experience with Laravel I remember some big debugging session where I tried to find out how things worked. I digged deep into the internals of the framework to understand how it works under the hood instead of just knowing the things I need to know in order to get the job done. Sure the first approach would have been easier, but for later issues I know how to solve problems because I know how things work. So even if you are now in the need of refactoring your whole side project, you have learned some serios skills. Sure, picking the fastest way to get the job done is not bad. But on the long term, the harder approach might actually help to to get the job done faster.

Sure, you might have done it the wrong way, when you tried to fix the problem on your own. There might be an abstraction of the language or framework that makes things easier. You could have used it right away, but now you know a bit more about your technology and how it works. It's still a win.

## Your sideproject is no system critical infrastructure

But there is still the question whether you should refactor your whole codebase or not. I would say it depends. It's a pretty personal question. I personally would always try to refactor it. If the result is not worth the effort you can limit your refactoring efforts to the basics. But what you should keep in mind is that your side project is no system critical infrastructure.

Lets be honest, most of us start a side project without actual planning. We got this idea and start coding right away. No Use-Case analysis. No UML class diagrams. Maybe some component designs, but even this happens pretty rarely for side projects only speaking for me. The main purpose of side projects is to have fun. We are not building the backend of any billion dollar enterprise here. These projects are not made to be like that. Side projects should give the developer the freedom to do whatever they want without any restrictions in component design or even best practises. These projects are made to make fun.

So please stop overengineering your side projects. If you are realistic, the main users of such a project will be you and your friends in most cases. There is no need to think about a microservice architecture in order to scale to 1.000.000 users at the same time. But if you like thinking about these problems go ahead and do so. 

## But should I read the docs?

Earlier in this article I have said, you should not read the docs. This is not completely right. Sure, you should definetly read the docs to get a basic understanding of how everything works. What I meant is, that you should not read the whole documentation in detail in order to prepare starting your project. 

Over the years I have developed my personal approach on how to use documentation of new projects. First I think about what I will need first. In the case of my side project it was Routing, basic REST-APIs and database interaction. So I sat down and started to read the docs superficial in order to get an idea of how things work. Then I start working on my project.   When I run into a problem then, I first try to solve it on my own. Through this mechanic I learn how the framework works. For example I do not lookup the documentation on how to get a search query parameter from the HTTP request URI. I take a look at the Request object that is handed over to my controller and check out its API whether this could help. Through this mechanic I do not only learn how I can retrieve a search param from the URI, but also how the API looks in general to be prepared for future problems. 

This might be the harder and more time consuming approach in the first place. But it will pay you off later. You see, there is always the shortcut to read the documentation or go on stack overflow or nowadays use ChatGPT or any other chatbot to solve your problem. But in your career you will also have to work with technologies that are not that well known or documented. In these cases you need to have knowledge of how the framework/language works internally in order to solve some of the problems. 

Let me give you an example for that: In my professional career I am currently working a lot with the PHP framework Symfony. It is pretty well documented and easy to start with. I would also say it has a pretty strong learning curve, because it simplifies many things pretty well. But like in any other frameworks it can get pretty complex. In of of the projects I had to work with a library that instanciates an admin dashboard. I wanted to override some form submission behaviour. The problem now was, that the Symfony docs does not show how to do this, because the admin dashboard library puts an extra abstraction layer on top of the Symfony API. Also stack overflow would not be that helpful, because this is not a common usecase to override this form submission behaviour. I had to know how the Symfony API works internally in order to hook into the form submission process and do the modification required. Without learning Symfony the hard way, I would never have been able to do that. 


## Conslusion

But what can you learn from all this? Side projects main focus is to have fun. You should not commit yourself to some restrictions you gave yourself. They are ideal to learn something new, because they are seperated hard commitments which gives you more space to do some experiments or make your mistakes and learn from them. And yes, your code will look pretty shitty and you will need to refactor it. But take a look at your first projects with the technology your currently most proficient with: Aren't they pretty shitty too? You always improve. And if you want to you can refactor your project afterwards with the new experience and expertise you have gained so far.

The second takeaway from all this is, that you should definetly read the docs. But you should also challange yourself. Don't make it too easy for yourself. If learning a new technology was easy for you, you didn't really learned something. Sure things might be really similar, but if things were no different, they are the same. So try solving a problem without reading the docs or asking a chatbot, but try to find out how things work and how you can use them. This leads in a matter of fact to more expertise than just reading the docs, because you actually know the thing and know how it works. You are experienced with it and not only read about it. 

So never stop learning and never stop challanging yourself, because this would lead to not learning anything. Failing makes you better at programming than reading.

An motivational quote for you:

*Just let them know that we have a finite amount of time on this planet and you can be viciously mediocre or you can get the fuck after it.* ~ idk who said that
