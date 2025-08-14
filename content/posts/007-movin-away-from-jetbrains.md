---
title: "Why I start avoiding Jetbrains for my personal projects"
date: 2025-08-14T1:00:00+01:00
tags:
  - jetbrains
  - sideprojects
comments: true
---

I’ve been using JetBrains IDEs since 2018. In fact, the very first line of code I ever wrote was inside [IntelliJ IDEA](https://www.jetbrains.com/de-de/idea/), and I still have a soft spot for it. Over the years, I’ve spent countless hours in JetBrains environments — whether it was IntelliJ for Java, PyCharm for Python, or WebStorm for front-end work. Their tools are seriously powerful, and I honestly still enjoy working with them.

But recently, things have started to shift.

Over the past few months, I found myself reaching more often for lightweight editors instead of firing up a full-blown JetBrains IDE. It wasn’t a conscious switch at first—more like a gradual drift. But eventually, I started thinking more critically about my workflow, the tools I use, and what actually fits best for the kind of personal projects I’m working on now.

In this post, I want to share that journey with you: the decisions I made along the way, what I learned from using both types of tools, and ultimately why I don’t rely on JetBrains software as much as I used to.

## Why Jetbrains at all?

When I first started using JetBrains products, I was just another bloody beginner trying to make sense of programming. Back then, I had no clue what I was doing, and honestly, JetBrains IDEs were a huge help in getting me off the ground.

They made it really easy to explore the basics of a language — how it’s structured, how it works, and what’s even possible. I still remember how convenient the project templates were. As a beginner, having those ready-to-go setups was a lifesaver. (Although, to be fair, I haven’t touched one of those templates in almost four years now.) Another big help was the integrated documentation support. Being able to look things up right inside the IDE made learning so much smoother.

As I gained more experience, I started thinking beyond just writing code. Suddenly, tools for working with Git, managing databases, or debugging became a lot more important. And while there were always editors or extensions out there for each of those things, JetBrains IDEs were the only ones that offered all of them in one place — and at a surprisingly high level of quality.

Let me show you what I mean using PhpStorm as an example.

**Git Integration That Just Works**

If you’ve ever worked on a team or maintained multiple branches, you’ve probably run into merge conflicts. JetBrains’ Git tools—available in all their IDEs are hands down the best I’ve used for handling them. You get a clear visual diff, an intuitive 3-way merge view, and the whole process just makes sense. Could I resolve conflicts by hand? Sure. But this tool saves time and reduces mistakes, which makes it a no-brainer.

**Framework Awareness**

As a PHP developer, I spend a lot of time with frameworks like Symfony and Laravel. PhpStorm doesn’t just understand PHP — it understands the ecosystem around it. It recognizes things like service config files, offers templates for REST controllers or repository classes, and even integrates with tools like PhpStan or PhpCsFixer. It can apply formatting automatically based on the rules those tools define, which is a small touch that adds a lot of value.

**SQL Support That Goes Beyond Highlighting**

Writing SQL directly in your code? PhpStorm doesn’t just highlight the syntax — it validates your queries based on your selected database type (PostgreSQL, MariaDB, SQL Server, etc.) and even against the current schema. That level of context-aware support is a huge productivity booster.

**Built-In Database Tools**

Speaking of databases: the built-in database browser is fantastic. You can inspect tables, edit schemas, and run queries right inside your IDE. You don’t need a separate tool like Adminer or pgAdmin for most tasks. Everything is right there — and it just works.

**Dev Containers, Debugging, and Language Versions**

PhpStorm also supports dev containers, which is super helpful for working in isolated environments. And debugging with Xdebug? Seamless. Yes, other IDEs can handle this too, but there’s something about how JetBrains presents and manages these tools that just feels... right.

One feature that really made my day recently is the way PhpStorm handles different PHP versions. Need to target 8.2 instead of 8.4? You can set the version, and the IDE will adjust its rules and suggestions accordingly. It’s a great way to catch compatibility issues early.

**VIM Mode & Other Small Touches**

I also use VIM motions, and having solid VIM support baked into the IDE is just another cherry on top. I know editors like VS Code offer this too, but again — JetBrains just seems to do it a bit better.

And of course, language-specific features like managing different Java versions in IntelliJ are super well-executed too. Honestly, there are so many features I love about JetBrains IDEs that I could probably write an entire post just listing them out. But that’s not really the focus here. The point is: JetBrains IDEs are seriously powerful, well-engineered, and full of thoughtful features that make development easier.


## Why use something else?

As much as I love JetBrains products — and I really do — they're not without their downsides. And over time, those downsides started to get in the way of how I like to work.

The first big issue I ran into was performance. I often work with very large codebases — 100k+ lines of code in some projects — and I usually have multiple windows open at once, switching between projects to look something up or cross-reference ideas. In that setup, PhpStorm can easily eat up 8GB of RAM, if not more. And that’s not even counting what the rest of my system is doing.

Then there’s indexing. Ah yes, the blessing and curse of JetBrains IDEs. Don’t get me wrong, being able to search through an entire project in milliseconds is amazing. That part of the experience is gold. But in larger codebases, the indexing process itself is painfully slow. Sometimes it takes several minutes to finish, and during that time, the entire IDE becomes sluggish. On top of that, I’ve even run into occasional crashes under heavy load. Maybe it's just me, but it's extremely frustrating when you're ready to dive into work — and instead you spend five minutes staring at a progress bar or restarting the IDE after a crash.

Somewhere along the way, especially after diving into Rust, I started to care more and more about performance. Rust sort of rewired my brain for thinking about efficiency. It made me appreciate speed and simplicity in my tools, just as much as in my code.

That’s when I tried RustRover. And... well, it wasn’t great. At least not when I first used it. It felt slow, and some Rust features like macro recognition or autocomplete just didn’t work as expected. I’ve heard it has improved a lot recently, and I’m sure it’s in a much better place now. But that early experience left a mark.

Eventually, a friend of mine recommended [Zed](https://zed.dev/), and I decided to give it a shot. The start was rough, not gonna lie. I was missing a lot of the features I had taken for granted. Even proper Git integration wasn’t available at first. But instead of going back to what I knew, I leaned into the challenge. I started using the raw Git CLI — and surprisingly, it was fun.

Over time, I began to appreciate this more minimal setup. I didn’t need an IDE telling me everything. I didn’t need deep debugging tools or integrated database inspectors for my personal Rust projects. What I did need was a fast, stable, and distraction-free environment. Zed, with just a few plugins for Rust and React, turned out to be exactly that.

No heavy indexing. No unexplained crashes. No unnecessary abstraction. Just my code, my terminal, and whatever tools I choose to plug in.

I slowly realized that for personal projects, I don't need everything JetBrains offers. I don't need dev container integration, live SQL validation, or built-in PHP version managers. It's all useful stuff, but in my current workflow, it feels more like bloat than help. This lightweight environment gives me a sense of control I hadn't felt in a while. It pushes me to understand the tools I'm using, rather than relying on an IDE to smooth out the details. And that’s something I’ve come to really value.

## To what will I stick in the future?

To be honest, this hasn’t been a simple or clear-cut decision — and even now, I’m not 100% sure where I’ll land long term.

For work projects, I’m definitely sticking with JetBrains tools. There’s just no replacement (yet) for the kind of power they offer. Full-text search across massive codebases is something I rely on daily, and the deep debugger integration, real-time SQL validation, and seamless Git support are must-haves in my day-to-day workflow.

A lot of the projects I work on involve multiple Git repositories—sometimes even split across submodules. Managing that level of complexity manually would be painful. JetBrains makes it manageable. And when it comes to resolving messy merge conflicts, their visual merge tool continues to be a lifesaver. It’s one of those features that, once you’ve used it, you never want to give up.

But for personal projects, the story is different. I want something lightweight. Something focused. Something that lets me just write code and enjoy the process without waiting for indexing or watching my RAM usage creep toward double digits.

That’s where Zed comes in. As long as it keeps supporting Rust and React well — and stays as clean and fast as it is now — I’m happy to use it for my personal coding. It’s minimal, fast, and gives me the kind of low-level control that makes the whole dev process feel more “hands-on”. It's just the code. Everything else I manage my self in my terminal emulator.  No extra abstractions. No bloat. Just the essentials.

That said, I want to be clear about one thing:
I’m still very much in love with JetBrains. In my opinion, they’re the best in the industry at what they do. Their products are thoughtful, powerful, and built with real developers in mind. They’ve helped me grow from a total beginner to a confident, professional developer — and they’ll always have a place in my heart.

So while I might not reach for a JetBrains IDE every time I spin up a personal project, I’m not going anywhere. For the big stuff — the mission-critical, get-things-done kind of work — JetBrains is still my go-to.

And I kind of love this balance.
