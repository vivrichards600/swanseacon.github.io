---
layout: post
title:  "Adam Tornhill - There's More to Code than Code"
date:   2015-05-05 12:18:18:00
isStaticPost: false
---

#### There's more to code than code

Our software industry is good at exploring new ways to do things. If you've been around for a while you've probably seen your fair share of trends come and go. These trends are reactions to past failures. We push the pendulum from one extreme to the next. Yesterday's silver bullet is tomorrow's legacy code. Right now microservices are all the rage. In a few years we'll see a counter reaction as we discover that the complexity is still there, only now it's distributed as well.

In our rush to improve we often miss the most fundamental component of any successful software design: the people who built it. It's my firm belief that if we want to truly improve as an industry, we need to understand the interaction between people and code. How our code affects us and how we, as an organization, affect the code we write.

Until now, this traditionally softer side of, well, software has been left to subjective judgments. Expert judgments, perhaps, but nonetheless at risk for cognitive and social biases. What if we could guide those decisions with objective data instead? What if we could get a social view of our codebase? 

We don't know what the future may hold. But we'll be well prepared for it if we can understand where we, and our code, stand today. Let's explore that direction.

#### A software architecture is a social design

First of all, it's impossible to separate technology decisions from people; Any software architecture is as much a social design as it is a technical one. That's a good thing because it means we, as developers, can optimize for what matters the most.

But most of the time we aren't designing new software architectures. We have existing systems that we need to maintain, improve and evolve. This is challenging enough from a technical point of view. So what would it mean if we add a social axis too? Follow along and explore an alternate reality where we get the information we need to make both technical and social decisions.

#### Move beyond code

Pretend for a moment that you join a new organization. Like most companies in our industry their codebase is a mixed bag. Some parts look good, you're even tempted to say "elegant". Others are more like a scary monster riddled with "temporary" solutions, workarounds and important business logic mixed together with seemingly random chunks of accidental complexity. How do you start to make sense of it? Which parts are the most important? What do you need to understand first? Where are the key components? And, who do you ask when you want to understand why a 'userId' field is "re-used" to represent a time-stamp in some interactions but not others?

Now, let's pretend for a moment that you are handed a complete map of the system. You notice immediately that it's not your typical diagram of wild boxes and cylinders connected by bold dashed lines. Instead it looks more like a topography that shows the distribution of complexity in the codebase together with information on the relative importance of each part. You're told that the map is generated from how the team has actually worked with the codebase, so you know it's closer to reality than what most documentation is. Sweet - now you know which components you need to grasp first and where the scariest parts are. That drives your learning.

In addition you get a view of the typical change patterns in the system. You see that each change to the GUI leads to a predictable change to a stored procedure in the database. That's good to know. It seems like an architectural principle, yes - a questionable one, but important to know about nonetheless. You speculate that this information could be used to highlight technical debt in the codebase; If different sub-systems need to change together, doesn't that mean there's a missing abstraction? Why are they so tightly coupled in time? Wow - this information really helps you ask the right questions.

But why stop there? Let's say you get a second map as well. If the first map showed the geography of the system, this second map illustrates the knowledge distribution. It's a map that immediately points you to the developer that knows the most about a certain module or sub-system. You realize that you no longer need to haunt the halls of the corporation, be sent from door to door to track down someone able to answer your question. Instead you just look at your map and know who you should communicate with. You realize that the information isn't perfect - abstractions of complex systems never are - but it works surprisingly well in practice.

#### Explore the social side of your codebase

Once you have all that information you notice that you can do so much more by combining it. Let's see: you know about the change patterns in your codebase. You also know about the knowledge distribution in the code. Hmmm, that's both technical and social information there. If we combine them, we should be able to spot organizational problems that we'd normally mistake for technical issues. How cool isn't that! And if we instead map out the knowledge distribution on a team level and then look for change patterns that cross those team boundaries then, well, we'd finally have a way to measure how well aligned we are with Conway's Law. That would be powerful stuff. And yet it just feels as a starting point. You know that you can do so much more with this data.

#### Turn the vision into reality

I hope you enjoyed our thought-experiment. Wouldn't it be great to have access to those tools and techniques on your own projects? In the real world? On the 8th of September at 11:35 you'll see how [Treat Your Code as a Crime Scene](http://swancon.co.uk/schedule/#session-17) delivers that reality. It's a new way to view code that will change how you work with legacy systems. Join me on this fascinating ride!


#### Did you enjoy this post?

You can listen to more from Adam this September at SwanseaCon. 

[Treat your Code as a Crime Scene](http://swancon.co.uk/schedule/#session-17)