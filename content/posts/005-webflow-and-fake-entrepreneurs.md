---
title: "Working title"
date: 2025-04-01T1:00:00+01:00
tags:
  - cms
  - entrepreneurship
  - rage
  - agency
comments: true
---

I’m currently quite active on social media, and more and more often I come across people on platforms like TikTok or X talking about how they’ve started a Webflow agency or are building the next SaaS or enterprise application for their clients. In most cases, that’s perfectly fine — experienced professionals sharing what they’re working on. Pretty cool.

But lately, I’ve been seeing more and more people who really trigger me.

Many of the people you see on social media might initially seem to offer a great deal — but if you take a closer look, their services are often quite poor. Sometimes, they even lie straight to your face.

## A bit of background information

Before we dive in, you need a bit of background to understand what really matters when building a website or a custom application for clients.

Creating a website isn’t just about choosing a CMS or applying a fancy template. It’s about building a cohesive brand identity for the people you're working with. Let me walk you through the entire process.

When you receive an initial request to build a website, the first step is to understand your client’s actual needs. What is the primary purpose of the website? Is it to boost sales? Increase awareness of the client’s mission? Generate leads? This clarity is essential, because everything you build — from structure to content — should serve this core purpose.

Once that’s clear, you need to think about project management. You’ll have to estimate costs: hosting, legal services, ongoing maintenance, and your own work. Transparency is key. Explain how the price is calculated and why it is what it is — high, low, or somewhere in between. Identify all stakeholders and make sure the project's framework conditions are crystal clear. If you skip this step, your project is likely to fail due to misalignment and lack of agreement with the client. But once the organizational groundwork is laid, the “real” work can begin.

Next comes screen design. What pages are needed? What content should go where? What type of content are we even talking about? Which colors and design style suit the brand? Should it be modern, retro, minimalistic? Every design decision should serve the primary purpose defined earlier. And no — a random WordPress template does not fulfill all of your client's needs. Sure, templates can work in low-budget scenarios or when a generic solution is acceptable (which might be the case in 1% of all projects). But if the goal is to build something purposeful and custom, a template just doesn’t cut it.

Templates are too generic. They’re designed to meet many use cases at once, but not specifically yours. And let’s face it—most template-based websites look the same, which makes it hard to stand out from the competition. A better approach? Use a framework like Bootstrap as a starting point and customize each component to match the client’s individual needs. Use the grid system as your foundation, but then tailor everything to truly serve your client.

Also, choose a CMS or page builder that allows for custom extensions and plugins. Ideally, it should be open-source and self-hostable. Why? Because your client’s needs will evolve. Imagine you build a site for a barbershop. Initially, it's just about listing prices and attracting local customers. A year later, they want an online booking system. Or imagine your current hosting provider becomes insecure or non-compliant with data protection laws. In such cases, being able to migrate quickly is essential. Tools like Webflow, with their closed ecosystems and vendor lock-in to AWS, can be a serious limitation. A self-hosted, open-source CMS gives you far more flexibility and control.

Even after the content and layout are finalized, your work isn’t done. These days, SEO matters — a lot. Ideally, you should consider SEO from the very beginning, even before laying out your first design wireframes.

And when it's time to buy the domain, make sure the client owns it. Have them register the domain in their name and give you access only to the DNS settings — unless you’re explicitly authorized to register domains on someone else's behalf. This protects your client from vendor lock-in. Clients should stay with your agency because of your excellent service, not because you hold their domain hostage. Anything else is just unprofessional.

Then there's the legal aspect. At minimum, every website needs an imprint (Impressum) and a privacy policy. Don’t underestimate this. ChatGPT can’t reliably write these for you. Services like e-recht24.de can help, but in some cases, you’ll need a real legal expert to make sure your site is compliant. It’s always safest to consult a lawyer or someone well-versed in online privacy laws, rather than blindly trusting a generator.

And no, it’s not enough to just list your cookies in the privacy policy and install a free cookie banner. You must ensure that no external resources are loaded before a user gives consent. And if they decline, those resources must not be loaded. Most cookie plugins don’t handle this properly.

Here in Germany, there are three key laws you need to be aware of: the european GDPR (DSGVO), the BDSG (Bundesdatenschutzgesetz), and the BFSG (Barrerefreiheiststärkungsgesetz). Familiarize yourself with them and understand the limitations they impose.

When you're developing custom software for clients, the standards become even stricter. Your software must follow up-to-date security practices. That takes professional experience — or at least several years of serious hobby development. When I first started out, I lacked that experience, and I built some truly awful apps for other people. Thankfully, they’re no longer in use! Those applications were completely insecure, poorly architected, and a nightmare to maintain.

So, if you're building production-grade software for clients, make absolutely sure you know what you’re doing. It’s not enough for ChatGPT to know — you need to know. You should be familiar with architecture, design patterns, security protocols, databases, and more. If you’ve just finished university and your only programming experience is a Java course you had to take, that’s not enough to develop real software without a senior supervising you.

Start with personal projects. Get your hands dirty. Learn. And I don’t mean build a basic calculator app — go deeper. Learn how to design scalable, maintainable, and secure systems. Do that before you start building for clients. Otherwise, they’ll end up with a mess—and you’ll be the one stuck cleaning it up.


## So what are the people doing that triggers me

- Well I digged deep into these communities to find out what they are doing. I wanted tons of videos, read many tweets and even got invited to some discord servers.
- Well the most frustrating thing is that some people lie directly into your face. Its not something new that people on the internet lie all the time, but those people lie to attract new customers. 
- Let me give you an example: I won't give any names, but what you need to know is, that here in Germany there is a special corporate legal form called "UG". You can start it with 1€ capital, but with the limitation that you have to save 25% of your revenue to build your capital up to 25.000€. Then your UG is converted into an GmbH. 
- Why do you need to know this? Well there is a person out there that got lately a lot of attention on social media for posing with his cars. He said that he is running multiple startups and his most successful company is a software development agency that he runs since 2017, which made him a millionare through earnings. Fun fact, if you look up this company on north data, it is still a UG and got registered in 2021. So this company did not started in 2017 and did not make him a millionare. I assume he just said that to generate attention for his company to get new customers. And in my opinion this is the worst you can do.
- But right behind this is the fact that most of these new "webflow agencies" do not know, what they are doing. 
- During my time in these discord servers I got pretty well into how these people are working on there projects. 
- You remember what I said about building a website? Those people do not search for a purpose for the customer. They only do what in there opinion fits best to the company. No real project management. Costs are only estimated by a short description of the project. No details on how long each page would take individually. Often they also do fixed prices like 2000€ per website. 
- They just use one of the default templates or buy one that costs about 50€ and modify them to look like it matches the astetic of the customer. Spoiler: in most cases it does not.
- Many of them also vendor-lock in to tools like webflow, which do not have that much plugin support and it is hard to add real custom behaviour to the website. 
- They never heard about about SEO and they buy the domain for their customer under their own name. Might look fine in the first place, but actually it can be pretty frustruating for the customer if they want to switch to another agency. 
- When it comes to legal stuff, this is what triggers me the most. Those people either use just simple GDPR notice generators or AI to generate their legal texts for them. No further checks if there are actually no external contents loaded before you perform any action in the consent banner.
- Being unprofessional and selling bad services. Okay, you are just a bad agency. But not caring about the legal compliance of your products by using AI is very very very unprofessional. If you do exactly that, you should not be allowed to ever build anything for a customer ever again. 

- But this was only about websites. When it comes to building custom applications it gets even worse. I will make it short. Most of the people I talked to have absolutely no experience. They wanted some python tutorials online and how think that a bachelors or masters degree is worthless, because they already know everything to build a functional application. Some of those people I talked to even never heard the word password hashing. They thought it has something to do with choosing secure passwords for different applications. 
- Those people build production applications that do run in different companies or organisations they built the software for. No knowledge about privacy restrictions or software architecture. If it gets complex, ChatGPT is their way to go. 
- Its actually pretty sad from the perspective of a professional developer.


## So what would I do better?

- Well I was thinking a lot lately about opening an own agency for websites which is also one of the reasons why I decided to write about this whole topic.
- First of all the most important thing would be to invest in an expert in privacy and legal stuff. This is not only very important for me, but also for my customers.
- After that I would actually talk with the customer about their needs and build a custom website for their needs. No templates, no cost estimations based on nothing.
- If you really want to be a great agency to work with, you need a lot of time to fulfill the customer needs. It's not just building the website. You also need to host and maintain it, which can take a lot of time. 
- And this is the big problem. You just can't build a website that is legally bullet proof and fulfills the customer needs by 100% if it only costs 2000€. The minimum amount of money needed would be 5000€ for small websites. 
- And this is the main reason why I am not currently an agency owner. I do not have the time to properly provide good services for my possible customers. I know how much time it would take to build a good website. Therefore, it would be more expensive than the competitors websites, who do not put as much effort into those website as it would be needed to get a good result for the customer. 
- And this is why most of these agencies are still profitable, they are the cheapest on the market.
- Sure, your local barber shop does not need a fancy website to be successful, but if his website looks like every other barber shops website, the site is actually useless, because it has no USP (unique selling point).

## What can we do to avoid those people?

- Well to be fair, not every one man agency offering you a 2000€ website is bad. There are also many good people out there, who know well what they are doing. 
- But to seperate the good from the bad agencies we need to do some things. 
- The first, very unrealistic approach would be to require some sort of certification in order to be allowed to build websites for other customers like it is already established for other products. 
- For example, cars need to pass many security and quality checks before they can be launched into the consumer market. The problem with building websites is that it is accessible to anyone. Everyone can watch a two hour YouTube tutorial and start playing with webflow or wordpress and click together a mediocre website. But the end result is not really what most professional people would define as quality. The end customer of a car can say from his limited perspective, if a car is good. He can say if it is fast enough for his needs. But without any knowledge in mechanical engineering he is not able to say whether the engine is well constructed and will last long, or not. And the same goes with websites. The design might look good, but in the end it does not fulfill the customer needs or is just not GDPR compliant. Without any professional background the customer will never be able to measure the actual quality of a website properly. 
- And this is where certifications come in. If every person building websites for customers needs to be certified by some sort of institution in order to get the allowance to build websites, this would regulate the market and ensure that all websites build for customers are actually meeting quality and privacy standards. 
- But this is hard to establish, because it would require political actions. 

- The second approach would be to create awareness for this topic in the population. People should know, that a 2000€ website most likely does not meet the standards that a modern website should have. 
- The market would regulate itself in this case. More people knowing about this would have the effect of less people buying those crappy websites. 

- Same for building custom applications

- But to be fair I am not an expert in neither of these fields, altough I am member of a political party and have the basic knowledge of how the markets works. In the end I am not able to 100% ensure that those ideas would actually have an effect on the situation itself. So feel free to leave your own ideas and opinions in the comments.


- Just be careful if you are on the customers site. If your customer integrates you into the process of creating the website it can be an indicator for good quality. But take also a closer look at how the agency calculates it's prices and talk precise about how they do their legal stuff (GDPR, etc.), how they plan to design the website and how the whole domain thing is handled. If the agency is transparent with that this is also a big green flag. And hey, even if the agency is using a privacy notice generator this can still be a good deal, if the agency offers you a cheaper price and actively communicates that the price is less expensive because of this. Just be aware of what you need. Templates might also be fine at some point. Transparent communication is key when working with the agency. If your agency communicates transparently from the first day on how their prices are built and why there service is so cheap or expensive, this can actually be a good deal. But as always it is safer to be more careful whan less careful. 