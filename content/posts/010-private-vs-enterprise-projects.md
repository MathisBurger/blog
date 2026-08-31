---
title: "You don't need enterprise level architecture for your private projects"
date: 2026-08-31T1:00:00+01:00
tags:
  - architecture 
  - software
  - sideprojects
comments: true
---

- When building private projects, people often either use the most simple architecture, or start to overengineer it.
- Although both approaches are absolutely valid, I think we should find a compromise. 
- Let me explain to you why.

## How do private and enterprise projects differ?

- First we have to know the differences between those two types of projects.
- Enterprise and private projects differ significantly 
- Private projects are developed only by yourself. You decide the architecture, you write the code, you test it.
- In an enterprise context those tasks are split across multiple roles. Usually one software architect designs the architecture only
- He conducts interviews with stakeholders, derives functional requirements and application characteristics and designs the architecture with regard to those requirements.
- The developer usually only has to care about software
- Furthermore, enterprise projects have completely different requirements on scale and performance. 
- While enterprise projects are often used by thousands of people concurrently is your private project realistically maybe used by 5 persons (you and 4 friends).
- In those situations literally any modern architecture and technology scales well enough to serve you and your friends at reasonable performance. 
- In addition, private projects are way simpler than enterprise projects. You just do not build an ERP system, you maybe build some tool or app for a personal use case
but nothing for regional or global scale. 
- So now we know, that comparing enterprise projects to private ones is like comparing apples to strawberries. Both state good but thats about it. 

## Why do people still tend to overengineer?

- Developers love to try out new stuff. When building a private project we are not getting paid for it. 
- We are doing it for fun. Therefore, devs are attracted by the opportunity to try out new pattern or technologies. 
- Actually, thats how I started using rust. I was mainly using go for private projects and wanted to try out this new trendy language. 
- This does not only apply for programming languages but also for architectures.
- When working for money, we are usually tied for months or even years to a single architecture that our architect decided to implement.
- So private projects present the perfect opportunity to play around with other architecture styles.
- But this usually results in todo apps build with 20 microservices and three different messaging solutions. To be clear, that is a hyperbole but it often quite similar to that, maybe less extreme
- It is always tempting to overengineer stuff in our private projects. 
- But there are also devs who do the absolute opposite. They dont use any architecture at all for private projects and end up building either a layered architecture out of 
habit or end up with the big ball of mud antipattern.
- But that is fine too, as your private projects are only used by yourself and building software in your free time should primarily be a great experience rather than exhausting.
- So it is absolutely fine to stay that way.


## Should we stop overengineering?

- All this raises the question whether we should stop overengineering? No we should not. 
- But nevertheless, we should be careful what we do. Building too complex architectures as private projects can train bad habits. 
- Just because some framework is hyped right now, it is not instantaniously a good choice for an enterprise project.
- Developers who regularly overengineer their private projects with the latest technologies might subconciously feel the need to implement those technologies 
in their enterprise projects too. The book "Fundamentals of Software Architecture" by Mark Richards and Neal Ford illustrates a similar example. A developer loves scala and widely 
wants to implement Scala. In the end, he poisoned the whole team and two other developers wanted to leave. 
- So it is really important that you mitigate the risk do adapt such a habit


## So what should we do then?

- If you want to overengineer, just continue to do so. 
- Same applies for developing without any architecture. 
- If you like to be without any restrictions on your private projects feel free to do so.
- I like to find a compromise. Think a bit about architecture. You don't need to do a complex trade-off analysis. 
- Just think briefly about what you want and what suits this use case best.
- I recently discussed with a friend of mine an application idea. It was an application that received images and displays them. Furthermore, images should be available in other sizes as well.
- We discussed two approaches. Either you build everything as a blocking workflow. First upload the image to S3 and then resize it or you use messaging to asyncronously perform the resizing in the background.
- To be fair, for a personal project both these approaches are fairly reasonable. 
- What can we learn from this? We could have split the app into 3 other microservices, but we decided to do not. 
- We went with a compromise. Only if it is abolutely useful to do something, do it. 
- Also give some other conclusions.