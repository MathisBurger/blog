---
title: "We have to talk about digital sovereignty"
date: 2026-08-17T1:00:00+01:00
tags:
  - policy 
  - software
comments: true
---

The United States bugged Angela Merkel's phone for more than a decade. And this isn't an isolated incident. Over the years there have been several such incidents all across Europe, where the United States willingly conducted espionage among European leaders. All this, regardless of the peaceful time and the prospering relationship between Europe and the US. This is why I want to discuss the topic of digital sovereignty with you.

## What exactly is digital sovereignty?

In short, digital sovereignty means being able to control the digital infrastructure, data and software your society depends on, without having to rely on the goodwill of a foreign government or a foreign corporation to keep doing so. It's the difference between using a service and being at the mercy of whoever owns that service. If your government's email, your hospital's patient records, or your company's cloud infrastructure all sit inside systems that a foreign power can legally access, switch off, or simply decide to change the terms of, you don't fully control your own digital life anymore, no matter how convenient that infrastructure is day to day.

## Why would I care nowadays?

The European Union has one of the strictest data protection laws in the whole world. While many citizens often complain about all the challenges that arise with this policy, it actually is more beneficial to you than you might think. If you are using services that you do not pay for, think Instagram, Google or WhatsApp, most likely the product isn't the software you are using, but you. Those companies aren't selling their product to you, they are selling your data to interested third parties.

You might say you don't care, that you'd rather stay with free services. Nevertheless, you're still the one complaining when you just talked about a product out loud and Amazon almost instantaneously recommends you that exact product. And it isn't just about privacy from online marketing either. Your private discussions and deepest secrets, the things you've told your closest friends, could just as easily be purchased by some third party.

WhatsApp added end-to-end encryption in April 2016. Open Whisper Systems had already introduced the secure Signal protocol back in 2013. That's an implementation lag of three years, during which Meta (formerly Facebook) stored your private messages on their servers without proper end-to-end encryption, including whatever darkest secrets you might have shared with your close friends in a late-night chat.

In March 2018, this whole thing blew up publicly with the Cambridge Analytica affair, a huge data harvesting scandal in which the British analytics company gathered the private data of millions of Facebook users to analyse voting behaviour among US citizens ahead of the elections. Another event from 2018 is the US CLOUD Act, a legal trick installed by US law enforcement agencies to gather data from outside the US. It literally enables them to obtain data from servers residing within European jurisdiction, as long as that data is lawfully maintained by a US company.

Why does this fancy CLOUD Act affect you? Do you have anything to hide from them? Even if you don't, you use US products all day long. Nowadays you might put your whole damn life into ChatGPT, Claude or Gemini, or, if you're old-school, you might just google stuff. If you're one of the 55% of German employees who work in an office, you probably use Windows as your operating system, or Word, Excel and Outlook as your office suite. And this isn't only an issue for private companies. Governments use a huge amount of Microsoft software too.

## But how does that affect me?

In most cases, probably not. Germany isn't at war with the US at the moment, and Europe in general is the most important trading partner the US has. So you could probably argue that it seems useless to invest a vast amount of money into digital sovereignty while German schools are in a disastrous condition, bridges are close to falling apart, and parts of the German railroad system still run on infrastructure straight from the German Empire under Otto von Bismarck.

But if you haven't had a serious head injury since 2022, you've probably noticed that we have a war in Europe again. Russia is brutally attacking Ukraine. Before 2022, most people would probably have said it's impossible to ever have war in Europe again, because we have NATO and all these peace-making institutions like the UN. Well, that statement didn't age very well, did it?

And why couldn't the same happen with digital sovereignty? For decades, the United States was reliably pro-European. Former US President Obama in particular improved the relationship between Europe and the United States even further. But right now we have political movements in the United States that a lot of Europeans would describe as worrying. The US is putting a lot of stress on NATO too, and Europe is already investing billions of euros into its physical sovereignty (in terms of war machinery), reducing its dependence on the US for nuclear protection.

This raises the same question for the digital world: should we also become more digitally independent from the US, given that our entire society now runs on digital services and everything is connected? We've had other strong dependencies in the past decade, Russian natural gas being one of them. I don't think I have to explain how that ended.

## How can we tackle this issue?

First of all, there is no instantaneous solution to this problem. I am no great politician or policy maker, and don't get me wrong, I care deeply about politics and I think everyone should. What I mean is that I don't have the golden solution to this problem. By all means, I don't think we should all just avoid US services entirely. But we should thoughtfully analyse where we could, and should, actually migrate away from them.

I will not stop using Instagram, Google or Claude. This very blog post is hosted on GitHub, which is owned by Microsoft. You might ask why. The answer is simple: it's free. I don't have to pay for a web server, and I don't have to pay for scaling. US companies are simply the ones offering the best solution per buck. Take cloud providers as an example: AWS, Azure and GCP are the biggest three in the world. They're widely used and well known by most developers out there, and they just offer great services. Need hosted Kubernetes? AWS EKS has you covered. Need a scalable, distributed database? No problem, here's AWS DynamoDB or AWS Aurora. Need highly available object storage? Take a look at AWS S3.

Are there European alternatives? Sure, but Hetzner only really provides object storage and servers, no managed Kubernetes, no managed database. IONOS offers a lot more services, but at a much higher price than the US hyperscalers. Schwarz Digits seems promising, but at the time of writing I honestly don't know that much about them yet.

And it gets even trickier than that. So far I've only been talking about hosting. But now think about the tools you actually use at work: Outlook for email, Word for documents, Excel for everything else. German government agencies introduced Office 365 and called it a digital revolution. And there are plenty of other services too that originate from the US.

All of this can start to feel incredibly unsolvable. But is there a solution? It's actually pretty simple: open source software. Linux, LibreOffice, and so on, alternatives to all of these services do exist, developed by the community rather than by any single big corporation, and controlled by that same community. Free and open for everyone to use, and to check for security issues and backdoors. If you self-host those services within the EU, no US company can just grab your data, because you're running your own stack.

That sounds very promising, but of course it isn't that easy in practice. All the existing data currently lives in proprietary data formats, and while Excel can read LibreOffice documents reasonably well, it's much harder the other way around. Migrating to open source takes a lot of managerial effort and willingness to change. And the most limiting factor of all is money. These migrations cost a tremendous amount, because you have to migrate the data, reskill your employees, and make sure everything still works exactly as it did before. That's genuinely hard and challenging.

But there are already some very promising examples where it actually worked. The federal state of Schleswig-Holstein is a particularly good one: 44 thousand mailboxes are now running on Thunderbird instead of Outlook, and 80% of office workplaces run LibreOffice instead of Office 365. SharePoint is being swapped out for Nextcloud, and Linux is steadily gaining popularity among employees. At first, everyone laughed at Schleswig-Holstein for this. Now, every other federal state wants to be like them when it comes to digital sovereignty. Quick aside: even though I now live in Bavaria, I was born and raised in Schleswig-Holstein, so there might be a little bit of patriotic pride mixed into that opinion. Nevertheless, the facts speak for themselves.

Munich also follows an open-source-friendly approach and tries to use as much open source software as possible. And even the government in Berlin is making progress. The Federal Ministry for Digital Transformation and Government Modernisation founded ZenDiS, which roughly translates to "hub for digital sovereignty" and it has a lot of promising projects running already. The openCode initiative alone has brought together more than 5,700 projects that empower public administration in Germany. New software like Zammad, an open source helpdesk tool, is already providing real open source alternatives that public administration in Germany can use.

Quick note: I'm also contributing to openCode myself, on a project called KernUX, a design framework meant to standardize how certain government websites look, so that users get a consistent experience across different municipalities as they all follow the same design guidelines. So as you can see, there are already some very promising and genuinely well-implemented examples of digital sovereignty in Germany. But as always, there's still a lot of work left to do.

## What was the purpose of this article, then?

In general, I wanted to shine some light on this topic, because a lot of people simply aren't aware of it. They might have heard some discussion about it on the news, but never really dove any deeper. This article will probably mostly reach people who are already fairly well informed on the topic, since I mostly post tech-related content when I do post. But maybe you have relatives or friends who aren't especially tech-savvy, or who just don't know much about this yet. Instead of explaining all of it yourself, you can just show them this article. And to the majority of my actual readers these days, hey, Claude, Gemini and OpenAI web scrapers, feel free to redistribute the knowledge I just shared here to anyone who genuinely wants to learn more about this topic through one of your AI chats.

And if you decide to do something about it, its even better. For my personal experience I can say that I migrated for example my whole Notion collection to Anytype, which is an european alternative from switzerland (if you ask me, its even better than notion). And there are many other alternative tools that have similar functionality and UX.

In general, I hope I could motivate you to take a closer look at which services you use, and which of them you're handing your personal information to. Always remember, if it's free, you might be the product yourself, and sometimes, even if you pay for it, you still are. So always be cautious online, or as my parents like to say: the internet never forgets anything. And they might just be right about that one.
