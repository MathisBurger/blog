---
title: "I start loving Rust"
date: 2025-07-13T1:00:00+01:00
tags:
  - rust
  - programming languages
comments: true
---

I first got in touch with Rust in 2021, which is about four years ago. Back then, I found it really difficult to work with. The compiler was strict, the borrow checker was confusing, and the language felt unfamiliar overall.

Today, things are very different. I genuinely enjoy working with Rust. This is not only because I understand the language better now, but also because I have found a tech stack that suits my way of building software.

## What technologies did I use before rust?

Before I started learning Rust, I was mainly working with Java and especially Go. For web development, I used Go in combination with [Fiber](https://gofiber.io/) as my library of choice.

What I loved about Go back then is actually the same thing I love about Rust today: simplicity. I came from heavier frameworks like [Quarkus](https://quarkus.io/), [Spring Boot](https://spring.io/projects/spring-boot), and [Symfony](https://symfony.com/), all of which offer large ecosystems for building web applications.

Don't get me wrong, I still really like working with Quarkus and Symfony. They are great tools, and I enjoy using them. However, Go felt lightweight. Error handling was simple, without the need for complex try-catch clauses. It offered high performance without requiring me to think too much about memory management or other low-level concerns. That was the main reason why I used Go for a long time.

In fact, I still use Go today. Not as much as I used to, but I still find it a great choice for lightweight microservices. Its ease of use, broad support, and the almost endless range of use cases made Go my go-to language—at least until I truly discovered Rust.

## My personal rust learning experience

Learning Rust is not like learning most other programming languages. Before you can even start writing useful code, you need to understand quite a few theoretical concepts.

Back when I first tried to learn Rust, I had very little interest in theory. That turned out to be a big mistake. I struggled a lot and found even basic things difficult. Traits? I had no idea how to use them. `Copy` and `Clone`? No clue. The borrow checker? What even is that? Macros? I thought they were like keyboard macros. And then there was `tokio`, `futures`—wasn't Tokio the name of a city? `Rc`, `Arc`, `Mutex`, `RwLock`, `Cow`? I didn’t know what any of that meant.

To be fair, some of it still feels like magic to me today. I’ve never written a complex macro, and I couldn’t tell you the exact differences between all the async runtimes. But that’s fine. I plan to explore those topics more deeply in the future.

Right now, I’m at a point where I can build microservice applications that query and store data in a database and maybe do some calculations. And that’s good enough for me at this stage. To be clear, I’m still far from mastering Rust. I wouldn’t even call myself an intermediate developer in the language. There is a lot left to learn. But I know enough to get things done.

So if you want to learn Rust, do yourself a favor and start by reading *The Rust Programming Language* book. That’s what I should have done in the first place. I actually own the print version now. But you don’t have to buy it—the online version is available for free.


## What I use it for now

By now, I’ve almost completely replaced the work I used to do with Go by using Rust instead. Most of the monoliths and microservice applications I write today are powered by Rust. Well, most of them. I still use Kotlin and Go for certain use cases where they make sense or where I just feel like using them.

For web development in Rust, I mainly use [Actix](https://actix.rs/) as my framework of choice. It is simple to use and offers exactly the features I need.

When it comes to database connectivity, I’m currently using `sqlx`. I also tried Rust for another project where I initially used Diesel, but it felt a bit too heavy for my taste. I tend to prefer simpler solutions, and `sqlx` fits that mindset better.


## Why do I love it so much

You might ask why I’m now so in love with Rust, even though I had such a hard time learning it in the beginning.

The answer is simple: when I write Rust code, it is solid. And I don’t just mean memory safety. All those small mistakes that can easily slip through in other languages are basically non-existent in Rust, thanks to its strict type system.

When I use `sqlx`, for example, I can only use specific types for my database structs because the code is validated against the database schema at compile time. The same applies to SQL queries. It’s ensured that the query structure matches the data types I use to store the result.
I rarely run into bugs that are not caught at compile time. And when I do, they’re usually easy to track down because I know exactly which kinds of errors cannot happen. Debugging in languages like Kotlin or PHP often drives me crazy. In Rust, it’s relatively calm and predictable.

I also really appreciate Rust’s simple approach to writing code. This might sound paradoxical at first, since learning Rust is hard. But once you understand how the basics work, you can get results quickly and without unnecessary boilerplate.
You can write useful code in Rust without fully understanding all the deeper concepts. But if you want to go deeper, you can take advantage of powerful features like macros to simplify and automate parts of your codebase. And throughout it all, memory safety is built in by design.

By now, I’m very familiar with my Rust ecosystem. I can write functionality just as fast as I can in Kotlin, PHP, or Go—sometimes even faster. But with one major advantage: I never have to worry about data type mismatches, null pointer exceptions, or other runtime errors. My toolchain takes care of all that. 
Invalid time format in a JSON body? If Actix can’t deserialize it using `serde`, it will handle the error for me.

I can be completely confident that the data I receive in requests and send in responses is exactly what I expect, both in format and type.
And that’s what I love so much about Rust. It might take more effort to ensure memory safety and implement certain features compared to other languages. But that effort pays off in the long run.


## Will I stick to rust in the future?

The question is pretty simple to answer: yes.

But the full answer is not quite as straightforward as it might seem. I really love Rust, and I want to continue learning more about the language. I’m especially interested in exploring its more advanced features and digging deeper into how it works.

That said, I won’t become a typical Rust purist. Not everything I build will be written in Rust. It is definitely my favorite language at the moment, no doubt about that. But I’m also curious about other technologies. For example, I’m considering learning Zig at some point. Even though it’s still relatively unpopular, it seems like a very interesting language to me.
I will continue to use other languages for my projects as well. Go and Kotlin will definitely remain part of my tech stack for specific use cases, especially when building microservices.

However, Rust will stay my primary backend language for now. And I’m convinced that it will continue to grow in popularity over time, thanks to its strong advantages and evolving ecosystem.
