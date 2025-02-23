---
layout: post
title: Startup Valencia Hackathon 2025
date: 2025-02-23 22:29 +0100
---
## Introduction

The days 21 and 22 of february 2025 I attended and won the ***"Startup Valencia Cybersecurity"*** hackathon. It was a hackathon of around 25 people divided in 6 groups. Each group had a challenge proposed by a compnay. Our challenge was to find a solution to stop frauds in ticketing websites. The company we had was ***Fourvenues*** which is actually the biggest ticketing company in Europe.

## What exactly was our challenge?

Nowadays it's pretty easy to find leaked bank cards on the internet which makes fraudulent actions pretty common. We got introduced to how the platform Fourvenues work and how the attackants were using it to their benefit.

Basically, you can create an organization user with real data(ex. Name, Bank account,ID)and then start creating fake events. These events will then be used by the attackers to use the stolen bank cards to buy an amout of tickets using automated scripts. This ended up in a lot of reports from the people that got stolen, and Fourvenues loses money and gets a fine.

## Our first ideas

The first approach was kind of messy. We didn't know the exact flow of how things happened when someone tried to buy a ticket, so that was the first thing we investigated. We realized that it was pretty easy to buy tickets, just using an email, a name and a bank account was enough to buy tickets which made the process of checking the cards pretty hard. We also didn't want to make a very difficult process of buying because then the customer would just change the platform and that would result in a los of customers. The first day ended and we went home not knowing what idea to choose.

## Final idea

After talking with some Fourvenues staff that was in the event and understanding everything we had to know, we came up with an idea. 

The idea was to use a technique called ***"Digital Twin"*** that consists in creating a double of the event which results in having 2 events, A and B. The attackers know that the event A is created and then they use that one to do the fraud. The event B is used to train the AI model so we can know what the real human interaction is with this kind of fake events. Then we also use a web scrapping set of scripts to gather information of the event before making it public. With this way we can know if an event is probably real or not, because if it's real or promoted by a famous celebrity, it will have a lot of interaction on social media, but if its fake, it will have 0 social interaction, no one will talk about it, and if they do, it's bad reviews. If the model can't verify if its real or not, it will put the event on hold and it will be reviewed manually. The more events occur, the more the model is trained and more accurate will be. The most important thing, is that all of this will hapen before the event is created. We want to delay the event publishing, so the way we do it is by sending an email to the organizer telling him that the event is being created and he will get emailed with the url when it gets published. That gives us enough time to gather all the information we need and then decide to block the event, publish it or put it on hold. Even if the event is fraudulent, with te Twin technique we will still publish the twin to train the model, but obviously that event won't accept the payments. Thanks to this we get a solution and we can train the model to be more accurate.

## Prototype

Even though we didn't have enough time to develop a prototype of the AI model, we developed a mini DEMO of the ***"fraud dashboard"*** that Fourvenues would see. The demo is available at my [github repository](https://github.com/ismafh/StopFraud_DEMO). 

Here's how the Control Panel would look:
![Control Panel](/assets/img/Captura%20de%20pantalla%202025-02-23%20230819.png)
There's a sidebar on the left with the "Fraude" option. We click on that:
![Fraud list](/assets/img/lista%20fraude.png)
We get a list with all the events and their actual status, tags and the reason.
Every event has it's own statistics and we can see them by clicking on the event we want:
![Event](/assets/img/evento.png)
We can see that every event has an engagement percentage, statistics per platform and the way people feels. We also get a report of remarkable things of the event at the left bottom box. 

## The end

This has been my first hackathon ever, and it has been a fun one. Very exciting from the first moment, all of my teammates were amazing and we did a pretty nice and organized project. I hope that the next hackathons are as good as this one :)

Thx for reading!! 
![winners](/assets/img/22022025-2024-12-25__HACKATON03208.jpg)