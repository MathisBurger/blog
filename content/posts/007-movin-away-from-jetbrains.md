---
title: "Why I start avoiding Jetbrains for my personal projects"
date: 2025-08-12T1:00:00+01:00
tags:
  - jetbrains
  - sideprojects
comments: true
---


- I am using Jetbrains IDEs since 2018. The first line of code I wrote was using [IntelliJ Community Edition](https://www.jetbrains.com/idea/).
- And I still really love working with their products. 
- But over the past few months I started to use some more lightweight editors. 
- In the following I will tell you about the decisions I made during that process and why I do not use Jetbrains sofwtare as often as back then.

## Why Jetbrains at all?

- The first time I started using jetbrains products I was just another bloddy beginner. 
- The Jetbrains IDEs were a great help when it came to understanding the simple structure of a language and exploring its capabilities.
- Also project initialization was much easier as a beginner, because of the simple project templates that the IDE offered. But to be fair I haven't used them for almost 4 years now.
- But the integrated documentation capabilites were a great help. 
- After I gained a little more experience I started thinking about other things than just writing code. Things like git, or database tools. 
- There were always IDEs that supported some of these requirements. But only Jetbrains IDEs supported all of those features at a pretty good level.
- Let me show you what I mean with PhpStorm as an example.
- When you use git, you will sooner or later run into merge conflicts when working with multiple branches and multiple people. The tool that Jetbrains integrated into all their IDEs is just perfect for this usecase. It displays the differences between two branches visually and allows you to merge them together in a very intuitive way. This feature improved my whole work process when it comes to git. Sure, I can also resolve merge conflicts by hand, but this makes it way better.
- Another useful integration is the support for different frameworks. As a PHP dev I am working a lot with frameworks like Symfony or Laravel. And PhpStorm knows the syntax of a service config file or has different templates for REST Controller or Repository classes. It also recognizes when you use tools like PhpStan or PhpCsFixer and helps you to auto apply your style formatting
- Also SQL Syntax highlighting came in very handy when writing SQL queries in code. But not only was the syntax highlighted but it was also validated against the configured database dialect (PostgreSQL, MariaDB, SQL Server, etc.) and the database schema in the database you have selected before.
- Now that we are talking about databases. PhpStorm (and any other Jetbrains IDE) includes databse inspection tools that can be used to view the content of the current tables, alter the schema or execute SQL queries. It is pretty useful when you have to work with databases and do not need an extra tool like Adminer or PgAdmin to manage your DB.
- Of course PHPStorm also has support for stuff like dev containers, which is also pretty useful. Furthermore, debugging using xDebug is also very simple and works just fine. Sure, other IDEs can do this too. But I somehow like the Jetbrains interface very much.
- An feature that also really made by day is the differenciation between different language versions. For example are there slightly differences between php 8.4 and 8.2 when it comes to defining constants. PhpStorm offers you the functionality to select which language version you are using and then uses a different set of rules for you. So you can always check whether your code would also run on a different php version.
- The last feature that came in pretty handly lately is support for VIM motions. Sure, there is also support for text editors like VSC. 
- As I already said, sure other IDEs also have some of those features I love so much about Jetbrains IDEs, but jetbrains implements them with a certain level of perfection. Everything works just fine.
- Of course there are also some language specific things like managing different Java versions directly from IntelliJ. Those are pretty well engineered too. But there are two many good features and things I really like about Jetbrains software. They can't be named in a single blog post. And this is also not the focus of this post. 

## Why use something else?

## To what will I stick in the future?

- Jetbrains full text search is really nice. 
