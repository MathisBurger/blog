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

I spent a lot of time digging into the communities I mentioned earlier, trying to understand how those one man agencies actually work. I watched countless videos, read endless tweets, and even joined a few Discord servers to see things from the inside.

The most frustrating part? Some people blatantly lie to your face. Now, sure—it's nothing new that people lie on the internet. But these folks are doing it to win over new customers. And that’s what makes it different.

Let me give you an example. I won’t name names, but here in Germany, there’s a special corporate legal form called a “UG” (Unternehmergesellschaft). You can start one with as little as €1 in capital, but you're required to save 25% of your profits until you reach €25,000. Once you hit that amount, your UG can be converted into a GmbH (a more robust corporate form).

Why does this matter? Well, there’s someone on social media who recently gained quite a bit of attention by posting flashy pictures with expensive cars, claiming he’s been running a successful software agency since 2017 — one that supposedly made him a millionaire. But if you check the public records on North Data, the company he’s referring to is still a UG and wasn’t even registered until 2021. So no, it didn’t start in 2017, and no, it didn’t make him a millionaire. It's all just a tactic to gain attention and attract new customers — and in my opinion, that’s as shady as it gets.

But the real issue goes deeper. Most of these new “Webflow agencies” have no idea what they’re doing. After spending time in their Discord servers, I got a pretty good sense of how they actually work.

Remember what I said earlier about building websites with purpose? These people don’t even ask what the website is supposed to achieve. They just create something they think fits the client's brand. There's no real project management. Cost estimates are based on vague descriptions with no breakdown of how long each page or feature will take. No clear cost structure, no distinction between hosting, maintenance, and development. In many cases, they offer fixed prices—like €2,000 for a full website—without any real scope definition.

They often use off-the-shelf templates or buy one for around €50 and slightly modify it to "match" the client's aesthetic. Spoiler alert: most of the time, it doesn’t.

Worse, they lock their clients into platforms like Webflow, which offer limited plugin support and make it hard to implement truly custom features. SEO is usually an afterthought — if it's considered at all. And as if that weren’t bad enough, they even register the domains under their own names. That might seem harmless at first, but when the client wants to switch agencies, it becomes a nightmare.

Now let’s talk about the legal side — this is what really sets me off. These agencies either use generic GDPR generators or AI tools to spit out privacy policies and legal texts, with zero regard for actual compliance. They don’t even bother to check whether third-party content is being loaded before consent is given via a cookie banner.

Selling mediocre work? Fine — you’re just a bad agency. But ignoring legal compliance and relying entirely on AI to generate legal documents? That’s not just unprofessional—it’s reckless. If you operate like that, you should not be allowed to build anything for clients. But clients often buy into it anyway — because it’s cheap and they lack the knowledge to understand the complexities and limitations of professional web design.

And that’s just websites. When it comes to custom applications, things get even worse.

I’ll keep it short: most of the people I encountered have no real experience. They’ve watched a few Python tutorials and now believe university degrees are pointless because they “already know everything” about building applications. Some of them hadn’t even heard of password hashing. One guy thought it referred to choosing strong passwords across different apps.

These people are building production systems — used by real companies and organizations — with no knowledge of software architecture, no understanding of privacy regulations, and zero awareness of secure development practices. And when things get complex, they just ask ChatGPT.

From the perspective of a professional developer, it’s genuinely sad to see.


## So what would I do better?

Lately, I’ve been seriously thinking about starting my own web design agency — which is also one of the reasons I decided to write about this entire topic.

First and foremost, the most important investment would be in a legal and privacy expert. That’s not just crucial for me personally, but also for the protection and trust of my future clients.

From there, I’d take a truly individual approach with each customer: sitting down with them to understand their specific needs and building a custom website tailored exactly to those goals. No templates, no baseless cost estimates.

If you really want to run an agency that delivers meaningful value, you need to take time — lots of it. It’s not just about building a website; you also have to host it, maintain it, and provide long-term support. That all adds up quickly.

And here’s the core issue: you simply can’t build a legally sound, fully custom website that truly serves the client’s needs for just €2,000. The bare minimum for a small, well-built site is around €5,000.

This is exactly why I haven’t started my own agency yet — I just don’t have the time right now to offer the level of service I know would be necessary. I understand what it takes to build a truly effective, secure, and purpose-driven website. And that kind of quality takes time — and therefore money. The websites I’d build would naturally be more expensive than what most of the cheaper agencies offer, simply because I’d invest far more effort into getting the right result for the customer. But I also don’t want to compromise on quality. I want to deliver the standard I would expect myself if I were the customer. And if I can’t achieve that with the resources I currently have, then I’d rather not do it at all. I’d feel uncomfortable offering a lower-quality solution at a cheaper price—especially knowing it might not truly meet the client’s needs. But maybe that’s just my perfectionism speaking.

That’s also why these low-cost agencies remain so profitable: they’re the cheapest option on the market. Sure, your local barbershop doesn’t need a highly sophisticated website to function. But if the website looks like every other barbershop’s site, it becomes practically useless — it offers no unique selling point, no reason to stand out.

## What can we do to avoid those people?

To be fair, not every one-person agency offering a €2000 website is necessarily bad. There are plenty of talented individuals out there who know exactly what they’re doing.

But in order to distinguish good agencies from bad ones, we need to take some action. One — admittedly unrealistic — approach would be to require some form of certification before someone is allowed to build websites professionally, similar to how other industries are regulated.

Take the automotive industry, for example. Cars must undergo rigorous safety and quality inspections before they can be sold to consumers. The issue with web development is that it’s extremely accessible. Anyone can watch a two-hour YouTube tutorial, start tinkering with Webflow or WordPress, and piece together a basic website. But the result often falls short of what a professional would define as a high-quality product.

Just like a car buyer might judge a vehicle by how fast or comfortable it feels, without understanding the inner workings of its engine or structural integrity, a client can think a website looks good while missing the fact that it fails to meet key needs — or worse, isn't even GDPR-compliant. Without a technical background, clients can’t reliably evaluate the actual quality of a website.

This is where certification could come into play. If anyone who wants to build websites for clients were required to obtain a certification from a recognized institution, it would help ensure that basic quality and privacy standards are met across the board. Of course, implementing such a system would require political will and infrastructure, which makes it a long shot for now.

A more realistic approach is raising awareness among the general public. People should understand that a €2000 website is unlikely to meet the standards of a modern, professionally built site. If more people become aware of the risks and limitations, the market could begin to regulate itself. Clients would be more selective, and low-quality providers would eventually get weeded out.

The same logic applies to building custom applications.

That said, I’m not an expert in either policy-making or economics — although I am a member of a political party and have a basic understanding of how markets work. I can’t claim with absolute certainty that these suggestions would have the desired effect, so I welcome your ideas and opinions in the comments.

If you’re a customer, be cautious. If your agency includes you in the development process and seeks your input regularly, that’s often a good sign. Also pay close attention to how they calculate their prices and how they approach legal compliance — especially GDPR. Ask detailed questions about their design process and how domain ownership is handled. Transparency in these areas is a major green flag.

And yes, even if an agency uses a privacy notice generator, that doesn’t automatically disqualify them. If the agency is open about it and offers a lower price as a result, that can still be a fair deal. Just be aware of what you need. Templates might work fine for some use cases. What really matters is transparent communication.

If an agency is upfront from the beginning about how its pricing is structured and why their service is either cheap or expensive, that’s a great sign. As always, it’s better to be cautious than careless.