---
title: "You don't need enterprise level architecture for your private projects"
date: 2026-08-31T1:00:00+01:00
tags:
  - architecture 
  - software
  - sideprojects
comments: true
---

When building private projects, people often either use the most simple architecture, or start to overengineer it. Although both approaches are absolutely valid, I think we should find a compromise. Let me explain to you why.

## How do private and enterprise projects differ?

First we have to know the differences between those two types of projects. Enterprise and private projects differ significantly. Private projects are developed only by yourself: you decide the architecture, you write the code, you test it. In an enterprise context those tasks are split across multiple roles. Usually one software architect designs the architecture only. He conducts interviews with stakeholders, derives functional requirements and application characteristics, and designs the architecture with regard to those requirements. The developer usually only has to care about the software itself.

Furthermore, enterprise projects have completely different requirements on scale and performance. While enterprise projects are often used by thousands of people concurrently, your private project is realistically maybe used by 5 persons (you and 4 friends). In those situations literally any modern architecture and technology scales well enough to serve you and your friends at reasonable performance. In addition, private projects are way simpler than enterprise projects. You just do not build an ERP system, you maybe build some tool or app for a personal use case, but nothing for regional or global scale.

So now we know that comparing enterprise projects to private ones is like comparing apples to strawberries. Both are fruit, but that's about it.

## Why do people still tend to overengineer?

Developers love to try out new stuff. When building a private project we are not getting paid for it, we are doing it for fun. Therefore, devs are attracted by the opportunity to try out new patterns or technologies. Actually, that's how I started using Rust. I was mainly using Go for private projects and wanted to try out this new trendy language. This does not only apply to programming languages but also to architectures. When working for money, we are usually tied for months or even years to a single architecture that our architect decided to implement, so private projects present the perfect opportunity to play around with other architecture styles.

But this usually results in todo apps built with 20 microservices and three different messaging solutions. To be clear, that is a hyperbole, but it's often quite similar to that, maybe less extreme. It is always tempting to overengineer stuff in our private projects.

But there are also devs who do the absolute opposite. They don't use any architecture at all for private projects and end up building either a layered architecture out of habit, or end up with the big ball of mud antipattern. But that is fine too, as your private projects are only used by yourself, and building software in your free time should primarily be a great experience rather than exhausting. So it is absolutely fine to stay that way.

## Should we stop overengineering?

All this raises the question whether we should stop overengineering. No, we should not. But nevertheless, we should be careful what we do, because building overly complex architectures in private projects can train bad habits. Just because some framework is hyped right now, it is not instantaneously a good choice for an enterprise project.

Developers who regularly overengineer their private projects with the latest technologies might subconsciously feel the need to implement those technologies in their enterprise projects too. The book ["Fundamentals of Software Architecture" by Mark Richards and Neal Ford](https://www.oreilly.com/library/view/fundamentals-of-software/9781098175504/) illustrates a similar example: a developer loves Scala and wants to widely implement it. In the end, he poisoned the whole team and two other developers wanted to leave. So it is really important that you mitigate the risk of adopting such a habit.

## So what should we do then?

If you want to overengineer, just continue to do so. The same applies to developing without any architecture at all. If you like to be without any restrictions on your private projects, feel free to do so. Personally, I like to find a compromise: think a bit about architecture. You don't need to do a complex trade-off analysis, just think briefly about what you want and what suits this use case best.

I recently discussed an application idea with a friend of mine. It was an application that received images and displayed them, and the images should be available in other sizes as well. We discussed two approaches: either you build everything as a blocking workflow, first uploading the image to S3 and then resizing it, or you use messaging to asynchronously perform the resizing in the background. To be fair, for a personal project both of these approaches are fairly reasonable.

What can we learn from this? We could have split the app into 3 other microservices, but we decided not to. We went with a compromise: only if it is absolutely useful to do something, do it.

## Conclusion

Private and enterprise projects live under completely different constraints, so it never makes sense to judge one by the other's standards. Overengineering your side projects isn't a problem in itself, and neither is skipping architecture entirely, both are fine as long as you're having fun. Just stay aware of the habits you're building, and try to make deliberate choices instead of defaulting to either extreme. A little bit of thought about what actually suits your use case goes a long way.