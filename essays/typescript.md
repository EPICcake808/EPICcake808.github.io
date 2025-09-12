---
layout: essay
type: essay
title: "Typescript and OOP: Foreign Concepts to Me"
date: 2025-09-11
published: true
labels:
  - Software Engineering
  - Typescript
---

<img width="200px" class="rounded float-start pe-4" src="../img/typescript/typescript.png">

Coming from a computer engineering background, TypeScript — and even just Object-Oriented Programming (OOP) in general — seemed so alien to me. I was used to doing things the hard way, so to speak. C, C++, and even Assembly felt like home: close to the hardware, where every pointer, register, and memory allocation was under my control. So when I was forced to learn Java and branch away from that comfort zone, I was thrown into completely new waters. And later, when I picked up TypeScript, I realized I wasn’t just learning a new language — I was learning a new way of thinking.  

OOP has never really felt natural to me. I come from a computer engineering background where most of what I did was imperative programming — C, low-level control, knowing exactly what the hardware was doing. When I first learned C++ OOP, I managed to pick it up, but it always felt kind of awkward, like something tacked on to the way I was used to thinking about code.  

Once I moved past C++ into languages that were built around OOP from the start, things got a lot harder. TypeScript especially threw me off. Its prototype-based inheritance felt completely foreign, almost like stepping into a jungle of new concepts. Learning it forced me to accept that OOP isn’t one neat, universal model. It shifts depending on the language, and figuring that out has been a struggle — but also one of the biggest ways I’ve grown as a programmer.

## Similarities between C/C++ and TypeScript

Even though TypeScript felt really different at first, there were a few things that felt familiar coming from C and C++. The biggest one was typing. In C and C++ I was used to being explicit about variable types, so when I saw TypeScript add typing back on top of JavaScript, it felt like coming home a little bit.  

Classes also looked familiar. In C++ I spent a lot of time writing `struct` or `class` definitions with constructors and methods, and TypeScript lets you do something that looks almost the same. The syntax was close enough that I could get started without feeling completely lost.  

Those little overlaps made the transition a bit less overwhelming. It reminded me that I wasn’t starting completely from scratch — some of the ideas I already knew still applied, even if the languages were coming from very different directions.

## Key Differences and Pain Points

The biggest difference I ran into was inheritance. In C++, it’s pretty straightforward: one class extends another, the compiler enforces the rules, and the hierarchy is clear. In TypeScript, the syntax *looks* the same — you can write `class Dog extends Animal` — but under the hood it’s all based on JavaScript’s prototype chain.  

That really tripped me up. I remember staring at examples like:

```javascript
Dog.prototype = Object.create(Animal.prototype);
Dog.prototype.constructor = Dog;
```

and thinking, “why can’t I just do Dog.prototype = Object.create(Animal)?” The idea that Animal itself was just a function, and its prototype was the actual place where inheritable methods lived, felt so strange. In C++, there’s no hidden object behind the scenes — the compiler just enforces the hierarchy directly. Here, it felt like I had to unlearn what inheritance even meant.

Memory management was another big shift. In C and C++ I had to think about pointers, allocation, and cleanup every step of the way. In TypeScript, I never even touch memory — garbage collection just takes care of it. It’s easier in a lot of ways, but it also means giving up the low-level control that I was used to.

For me, the hardest part hasn’t been types — coming from C, I’m always aware of them, and TypeScript’s type system felt natural right away. The real challenge has been adjusting to the prototype-based inheritance model. That’s where I’ve had to completely retrain the way I think about how objects share behavior.

## Athletic Software Engineering and WODs: A Great Way to Prepare

When it comes to athletic software engineering and the idea of ‘workouts of the day’ (WODs), the fast pace has been a real challenge for me. It’s not a rhythm I’m fully comfortable with yet, and trying to keep up has been a struggle. That said, my experience with online assessments (OAs) and technical interviews has shown me the value of this kind of structure.  

If you’ve ever used LeetCode, you know it’s a powerful tool for preparing for interviews. But it’s not always easy to sit down and grind problems without direction — the goals can feel vague or ambiguous, and it’s easy to lose motivation. What I appreciate about athletic software engineering and the WOD format is that it gives focus and accountability. Each “workout” provides a clear, specific task, and over time the repetition builds skill and confidence, just like physical training.  

For me, this structure turns practice into something more purposeful. Instead of endless problem sets, it feels like progress I can measure and build on — preparation that actually gets me closer to succeeding in interviews and, hopefully, breaking into the industry.

## Seeing into the Future

Looking ahead, I can see how these experiences fit together. Moving from C and C++ into TypeScript has pushed me to rethink how I approach programming, and learning OOP in a prototype-based world has stretched the way I think about design. At the same time, the structure of athletic software engineering and WODs has given me a framework for steady practice and growth, the same way athletes train day after day to get stronger. 

Even if my long-term focus is more on AI and machine learning, these lessons are still essential. Strong foundations in OOP and software engineering practices make it easier to build and maintain real systems, not just models in isolation. The discipline of consistent “workouts” builds habits I’ll carry into any technical challenge.  

I know getting into the industry is hard, but I can already feel how each small step — learning OOP, tackling WODs, staying consistent — is making me more prepared for the challenges ahead.
