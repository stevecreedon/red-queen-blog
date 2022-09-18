---
title: "InfoSec is just good business"
date: 2022-07-23T08:39:17+01:00
draft: false
tags: ["ISO 27001","Security Processes"]
categories:
  - InfoSec
cover:
  image: infosec-good-business.jpg
  relative: true
  hidden: false
aliases:
  - /posts/process-before-policy/
---
> *"**People who feel safe work harder and your biggest cost each month, <u>by far</u>, is wages not safety equipment.**"*
>
>  I learned this after graduating as a civil engineer. Now years later I'm an engineer in IT and it's pretty much the same for InfoSec. Yes sure it keeps evil hackers at bay but mostly it's just good management that gives your team more organised with much more time to move the dial forward and less time spent fixing & firefighting the unexpected. 

# & I write software

For the record, I'm an engineer that manages the development of websites. I'm not a security expert selling "InfoSec" services. Generally I take a dim view of all those tech security industry experts I see on [LinkedIn](linkedin.com) trying to scare me into buying their services. Much like the construction industry before I've learned that getting security right adds a level of organisational skill that small to medium businesses often lack. Done right this skill takes very little time out of the working week but knocks massive holes in '**failure demand**' - time spent  reacting to the unplanned events not developing the product you're selling.

My InfoSec experience comes from implementing [ISO 27001- Information Security Management](https://www.iso.org/isoiec-27001-information-security.html) but there are others such as [SOC 2]( reacting to the unplanned events). These standards help companies demonstrate basic competency in managing information security. I only say 'basic' because all my colleagues seem to think that implementing an InfoSec standard is tantamount to setting up a cyberwarfare unit within the business. The standards support good practices rather than specfic security technolgied and that's a great place to be. Like so many companies our data is of little interest to cyber-criminals so all of the InfoSec failures that have occured on my watch have been down to people making basic mistakes rather than the company being the target of a cyber attack.

# The Wrong Form

I worked for a startup as *'employee number three'* that quckly grew to 90+. In the early we had little or no process but when it came to monetising what we did we realised our potential clients were banks and government departments with more compliance and security departments than we had people.

In fairness most were quite pragmatic in what they expected from us. Our security tech was pretty strong for a company our size and background - we ran everything inside a VPC with only the bare minimum of the stack exposed to the web but we weren't that organised so every time we engaged with a new client I spent days filling in lengthy security questionnaires so that they could be sure we could be trusted with data.

This came to a head when I spent - quite literally - from 9AM one Monday morning through to 4.45PM the following Friday afternoon responding to a 700 question security questionnaire on a super clunky Excel spreadsheet. It was a merge of questions from various departments of a well-known high street bank and many of the questions were repeated in different words which was a really did make me question my sanity at times.

The following Wednesday I asked our Sales Director if he'd heard anything back from the bank. Five minutes later he was back "*You're not going to like this, they sent you the wrong form....*"

# The same questions 

Unsurprisingly these questions were pretty much the same from client-to-client. I'd been toying with the idea of writing some sort of security FAQ hoping that would stop me from having to fill in any more. & bounced the idea off one client's InfoSec manager that had been particularly helpful. His response: "Why not get ISO27001 ?, that'll keep us happy".

In the construction industry my company had made the decision to get the then 'kitemark' of quality BS 5750. Our CEO did want to be hire consultants that would spoon feed us into getting the kitemark, he wanted to learn and apply the principals of BS 5750. It wasn't easy but the transition made us a MUCH better organisation in the process. For the first time I actually understood what my job required of me; up until then I was a civil-engineer that, if asked, "civil-engineered" things. It felt right that we do the same thing in my present company for ISO27001.

# Not as good as I thought

We purchased a copy of ISO 27001 and its companion 27002 (ISO 27001 with examples). I gave myself the best part of two days sitting at the back of Caffe Nerro in Winchester purposefully reading through all 114 'controls' and trying not to be distracted by anything that moved.  Managing InfoSec is mostly about managing risk and each control is something you do to control risk.

I knew we'd fail one of the most obvious controls - "not keeping track of who has access to stuff". A quick check of our github account revealed we had four users - one with full admin rights - that we hadn't removed when they left the company. Sounds obvious I know but it doesn't happen by itself; we were all busy fools at the time & someone has to own the process to ensures it happens.

Reading through the document 90% of these controls fell into one of two categories:

1. We were already doing it but in most cases hadn't formalised the process.
2. We weren't already doing it but we really should and I felt a little uncomfortable that we weren't.

The other 10% just weren't relevant to our business ( ISO 27001 is as applicable to a high street shop as it was to a tech startup like ours ) and the standard is flexible enough to allow you to discount controls that don't make sense to your business.

Having responded to all those questionnaires and been subject to three security audits by 'experts' I'd been pretty confident about our Information Security capabilities but looking at the things we weren't doing I realised that we were only doing the obvious techy stuff like firewalls and private networks. Our focus had always been on the classic ( & with hindsight very naive ) "keep the bad guys out". In my time there we had four noteable InfoSec incidents and none of them were to do with black hat hackers trying to steal our data.

* We accidentally deleted a large part of production data (twice).
* We accidentally exposed private data to the web.
* Critical source code was accessed by a disgruntled employee that hadn't been removed from our systems.

ISO 27001 takes a much more grown up view of security,  which it terms "**CIA**":

* **Confidentiality** - keeping data secure.
* **Integrity** - keeping data accurate.
* **Availability** - making sure data is available when needed.

We were doing well with "**Confidentiality**" but completely overlooked both the "**Integrity**" and the "**Availability**". What struck me reading through all of these "**I**" & "**A**" controls is just how much they were common sense. Before starting a part of me feared that the ISO27001 would take us to a place of "Security Gone Mad" but the reality was quite opposite. It was just obvious adopting ISO 27001 would just make us a more organised & efficient business as well as a more secure one.

# We Built a Better business

Rather than give you a blow-by-blow listing of all the things we changed (I know the internet loves a list) I'll give you a taste of what changed.

We identified all the places we kept data - things like emails, documents, images as well as the more obvious database. We assigned owners to each data source who then checked how each was backed-up, who had access, was the payment information up to date or close to expiring ? Then we reviewed these on a quartelrly basis, each review took less than an hour.

In the perfect world we'd already have been measuring things like "failure demand" vs "value demand" so that we could see just how these changes impacted us but we were too busy being busy fools and just not that organised. 

I'm confident the changes were as profound as they were positive but I'm also a little ashamed to mention it because, well, it was always my job to make this happen. For the first time our people knew what to do which gave them a sense of ownership & teamwork that we just hadn't had. 

Fundamentally we began to feel in control rather than reacting to crises and like my construction workers way back we were working confidently on a stack that felt safe rather than one where we all trod cautiously in case something went wrong.

# Is ISO 27001 right for you ?

 In the mid to long run almost certainly yes. It is a lot of work so I wouldn't start unless you are determined to see it through to the end. Working back from a somewhat dry standard into actionable policies, procedures and processes doesn't happen naturally.

I have noticed that most companies share many of the same challenges so applying ISO 27001 does start to feel like re-inventing the wheel quite quickly.

That said, I do believe this kind of transformation is always worth it so I'm working on an opinionated framework that will give smaller businesses an 'opinionated' kick start. By that I mean a series of steps that get you to the benefits far more quickly than setting out on an all-or-nothing oddessy. When completed these steps will make the final transition to ISO 27001 (or SOC2) much easier as the fundamentals will be in place on paper and within the culture of your business.

The framework will be free so if you've read this and are interested then feel free to drop me a line.  