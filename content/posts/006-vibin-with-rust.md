---
title: "I start loving Rust"
date: 2025-07-12T1:00:00+01:00
tags:
  - rust
  - programming languages
comments: true
---

- I had my first contact with rust in 2021 about 4 years ago. Back then I had a really hard time working with it.
- Today I absolutely love rust. Not just because I know the language now a little better, but also because I found my ideal tech stack.
- I would like to share my experience with you and also get a little into why I prefer rust now over golang for my new projects. 

## What technologies did I use before rust?

- Before I started learning rust I was mainly using Java and especially golang. 
- Golang in combination with [fiber](https://gofiber.io/) as my library of choice for web development. 
- The thing I loved about golang back then is the same thing I now love about rust. The simplicity. I came from heavy frameworks like [Quarkus](https://quarkus.io/), [Spring Boot](https://spring.io/projects/spring-boot) and [Symfony](https://symfony.com/) that all have a big ecosystem for developing web applications.
- Don't get me wrong. I still love especially Quarkus and Symfony and enjoy working with them. 
- But golang was lightweight. Very simple error handling, no complex try-catch clauses. High performance without having to worry too much about memory management or else. And that is the reason why I was using golang for a very long time.
- Actually I still use it today. Not as much as back then, but I still enjoy using it for lightweight microservices. 
- It's easiness to use together with the broad support and nearly unlimited possibilities you could use golang for made it my language of choice before I really discovered rust.

## My personal rust learning experience

- Learning rust is not similar to learning other programming languages.
- You will need to understand many theoretical concepts before you can actually start writing code.
- I had no interest in theory back then, which later was a big mistake. I had a really hard time doing almost anything. 
- Traits? I didn't know how to use them. Copy and Clone? No clue? Borrow checker? What the hell is this? Makros? Like keyboard makros? tokio, futures? Isn't tokio a city? Rc, Arc, Mutex, RwLock, Cow? I dont't know what that is???
- To be fair, some of that stuff is still magic to me today. I have never written a complex macro or know the exact difference between all the async runtimes.
- I will discover that in the future by looking closer into it. 
- But currently I am at a stage where I would say I come around pretty well when it comes to just writing my microservie applications that query and store some data from the database and maybe do some calculations. 
- To be clear I am far away from mastering rust. I am not even on a intermediate level I would say. There is still a lot to learn. But I know enough to get some work done. 
- So if you want to learn rust, better start reading the rust book. This is what I should have done in the first place. 
- In fact I actually own it as the print version now. But you don't need to buy it. Just use the online version.

## What I use it for now

- I almost replaced the work I would have done with golang by rust now. All my monolith or microservice applications that I write are rust powered. Well most of them. Of course I still use Kotlin and golang for some stuff where I might wanna use it. 
- I mainly use [actix](https://actix.rs/) as my library of choice for web development. It is simple to use and has exactly the features I need.
- For database connectivity I am currently stuck with sqlx. But I also used rust for another project. But diesel was a little too heavy for me. I like it simple.

## Why do I love it so much

- Well you might ask why I now so in love with rust when I had such a hard time learning it.
- When I write rust code, it is solid. And I do not only mean memory safe. All those little mistakes you might make with 
other languages are just non-existant due to the strict type system. 
- When I use sqlx I can only use specific types for my database structs, because it is validated against the database schema at compile time. As well as all the SQL queries. It is ensured the query structure matches the data types I store the query result in. 
- I barely encounter bugs that are not catched at compile time. And when I do, they are relatively easy to find, because I know which specific errors cannot happen. Debugging drives me crazy in languages like Kotlin or PHP. But in rust it is relatively chill. 
- Furthermore, I really like the simple approach of rust. This might seem paradox at first, because it is hard to learn. But once you encountered how the basics work, it is really easy to get results fast and without unnessesary boilerplate code. 
- You can write code without understanding deeper principles of rust. But if you want to, you can go really deep and use some macros for your app to even simplify some things. And remember, all of this with memory-safety as a feature. 
- I am well familiar with my rust ecosystem now. So I can write functionality as fast as I can in Kotlin, PHP or golang. Maybe a little faster sometimes. But with the advantage of never having to worry about data type mismatches, null pointer exceptions or other runtime errors. My ecosystem covers them all. 
- Invalid time format provided in JSON body? If actix can't deserialize it using serde, actix will handle the error. 
- I can be 100% sure that the data I get as a request or return as a response is technically exactly what I want. 
- And this is what I love so much about rust. It might be hard to ensure memory-safety and sometimes implementing features would be way easier using other languages. But the effort pays off on the long run. 

## Will I stick to rust in the future?

- This question is pretty simple to answer: Yes.
- But the answer might the not that simple as it seems. I really love rust and I want to learn more about the language itself. I want to learn about the more advanced features.
- But I will not become a typical rust geek. Not everthing I build will be done in rust in the future. The language is my favorite language currently, no doubt. But I may also learn zig in the future and take a look at how much I like zig. Even if it is pretty unpopular currently it seems like a highly interesting language to me. 
- And I will also use other languages for my project. I will stick to golang and kotlin for some microservices for sure. 
- But rust will stay my primary backend language for now. I am also convinced it will grow even more in popularity in the future due to it's advantages and ecosystem. 