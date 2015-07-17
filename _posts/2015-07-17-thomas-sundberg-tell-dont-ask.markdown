---
layout: post
title:  "Thomas Sundberg - Tell, don't ask"
date:   2015-05-05 12:18:18:00
isStaticPost: false
---

#### Tell, don't ask

##### Why talk about 'Tell, don't ask' at Swanseacon 2015?

Objects that expose wrong information are complicated to work with. They force you to dig for the information you really need. It is easy to create a model where the users are expected to know a lot about the domain and therefore force them to dig deep into an object structure to get the information they currently need. This can be avoided if you strive for telling objects what to do and only ask them occasionally.

Asking an object for something may or may not result in a direct answer. If you get a direct answer to your question, it's usually not a problem with asking. But if you get another object back that you have to ask a more specific question and this object in turn returns yet another object that you need to inquire for the information you need, then you have a problem. A problem with code is that it is very tightly coupled. Objects are more or less tangled. Probably more. This may not seem as a problem if you know the code base very well, but it is unnecessarily complicated to understand how it should be used. A new developer will definitely have problems understanding the code base. It is also a very clear sign of missing abstractions. The initial object you asked for should have given you the answer to your question. If it doesn't have the answer, it should have asked some of its collaborators and then responded to your question. Not force you to ask for the proper collaborator and then ask the returned collaborator for what you really want to know. Possibly in many steps.

If you only tell objects what to do, it is a lot harder to tangle things together. It is also a lot easier to test. All you have to do is verify that the object you want to do something with has received a message that tells it what to do. This can easily be done with mocks that verify that a collaborator has been called.

Telling an object what to do instead of asking it for information forces you to focus on the interaction between objects. You must think a lot about the protocol between the objects.

Focusing on telling instead of asking is one technique to separate concerns and allows you to avoid making a spaghetti bolognese of your code base. Suppressing your chef ambitions when writing code is usually a good thing.

It turns out that seasoned developers sometimes don’t understand this concept. I have worked in a team where I found a code base mostly created by an supposedly experienced developer who, it turned out, either was too smart and could remember all connections between the objects or too stupid to understand that it was hard to grasp. It was a green field project that ended up with a lot of performance issues that were hard to resolve. The tangled code was not the main reason for the performance issues, but it didn't help when we struggled to resolve them. Changing a tangled codebase is difficult and it became unnecessarily difficult to re-write the parts that had performance problems.

Why do I want to talk about this at Swansea? Interaction between objects is the single most important thing in object-oriented programming. Unfortunately, some developers neglect it. I expect that there will be a lot of developers at a conference about Agile Development and Software craftsmanship. Some of them might need to be reminded about the Law of Demeter.

#### Did you enjoy this post?

You can listen to more from Thomas this September at SwanseaCon. 

[Tell, don't ask](http://swancon.co.uk/schedule/#session-13)