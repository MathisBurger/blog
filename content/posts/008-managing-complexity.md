---
title: "Why managing complexity in software engineering is the key to everything"
date: 2025-04-01T1:00:00+01:00
tags:
  -complexity 
  - software
comments: true
---

Everytime I faced a problem in the software engineering process, it was somewhat related to poor complexity management. 
You might not think it is related to complexity issues, but at some point it is.

# What is complexity exactly?

Complexity is a multi facade term. I won't use some encyclopedia description that persists of some hard to understand phrases in order to explain it. Let me give you some probaly relatable examples instead.

Everytime you wonder why the code looks like a mess its because you did not manage to know the complexity of the function beforehand and ended up building it without thinking about how to split it up or write it in a more readable way. 
If you read the Clean Code book you might know that you can write a whole philiosophy on readability of code. COmplexity is exactly that. Complex code is harder to read. and therefore also harder to understand. You can reduce complexity by splitting up your functions into smaller functions that do exactly one single thing. That reduces the complexity of each individual function to a minimum and makes the overall complexity more managebale and overseeable. 

 This also relates to the amount of parameters you can pass to a function. The more paramenters or complex parameters you have the more unpredictable is the actual outcome of the function is. 
 Lets compare those two functions 
 
 ```rust
 // Function one
 fn do_something(a: u32) -> u32

// Function two
fn do_something_else(a: u32, b: HashSet<Vec<HashMap<String, String>>>, c: bool) -> u32
 ```
 
 As you can see the second function is a lot more complex. We have three parameters of which the second one is a very complex datatype. Testing this is a nightmare. You won't even get close to an acceptable test coverage. And even if you get there, how do you ensure that actually the thing works as expected? 
 
 Ensuring the integrity of the whole software gets even harder when a function requires interaction with other classes or services. Its pretty straight forward to unit test a single class or even multiple classes independently. 
 It starts to get really tricky when you have to integrate together different components.

# Where is complexity management most important?

Most important is it to manage complexity when you have multiple services or components of a system that are loose coupled. You often don't know which service will communicate with which other service. It's mightmare to manage, debug and prevent. 

Let me give you an extreme example: Car software.

Modern cars are more a driving smartphone than out classic understanding of a vehicle. And they have one speciality that is a nightmare in terms of complexity management. They are highly configurable. I bet everyone has already opened at some point the website of a premium car manufacturer like Porsche, Audi, BMW or Mercedes and configured his dream car. But have you ever thought what this configurability means to complexity?

Just imagine how many different configuration options for seats there are: Normal or sport seats, heating or no heating, cooling or no cooling, massage or no massage, leather or fabric. All of those are almost freely configurable. Thats 2^5 = 32 different seats! And almost all of those options do have an effect on the underlying software. And now imagine all the other options you can pick in the configuration process. 

Without proper complexity management it's impossoble to ensure the car works as expected at all. Of course this is a extreme example, but there are other examples of applications that handle very loose coupled usecases that can lead to unwanted side effects. 

# How can I manage complexity then?

# Lets put it all together
