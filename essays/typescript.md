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

<img width="200px" class="rounded float-start pe-4" src="../img/tools/chatgptlogo.png">

Coming from a computer engineering background, TypeScript — and even just Object-Oriented Programming in general — seemed so alien to me. I was used to doing things the hard way, so to speak. C, C++, and even Assembly felt like home: close to the hardware, where every pointer, register, and memory allocation was under my control. So when I was forced to learn Java and branch away from that comfort zone, I was thrown into completely new waters. And later, when I picked up TypeScript, I realized I wasn’t just learning a new language — I was learning a new way of thinking.  

Transitioning to TypeScript meant re-examining everything I thought I knew about OOP. Classes in C++ felt natural — define a structure, hide implementation details, inherit when necessary, done. But in JavaScript and TypeScript, OOP isn’t “classical” at all; it’s built on prototypes, and behavior is shared in ways that initially felt counterintuitive.  

## Similarities between C/C++ and TypeScript

Even though TypeScript felt very different at first, I noticed some familiar things coming from C and C++. The most obvious similarity is typing. In C and C++ you always have to be clear about the type of your variables, and with TypeScript I got that same safety back after using plain JavaScript.  

Classes also looked familiar. In C++ I was used to writing `struct` or `class` definitions with constructors and methods, and TypeScript lets you do almost the same thing. The syntax is close enough that it didn’t take me long to pick it up.  

Those similarities helped me feel like I wasn’t starting from zero. I could lean on what I already knew, even if the languages were built on very different foundations.

## Key Differences and Pain Points

The biggest difference I ran into was how inheritance actually works. In C++, inheritance is straightforward: one class extends another, the compiler enforces the rules, and the hierarchy is clear. In TypeScript, the syntax looks similar — you write `class Dog extends Animal` — but underneath, it’s all built on JavaScript’s prototype chain. This was really confusing for me at first. I remember looking at examples like:

```javascript
Dog.prototype = Object.create(Animal.prototype);
Dog.prototype.constructor = Dog;
```

and wondering why I couldn’t just write Dog.prototype = Object.create(Animal). The idea that Animal itself was just a function, and that its prototype was where the inheritable methods lived, took me a while to wrap my head around. In C++, there’s no such thing as a “prototype object” sitting behind the scenes. The inheritance chain is enforced directly by the compiler, not by dynamic lookups at runtime.

Memory management is another big difference. In C and C++ I had to think about pointers, allocations, and cleanup. In TypeScript I don’t touch memory at all — garbage collection just handles it. It makes code easier to write, but it also feels like giving up the kind of low-level control I was used to.

Error handling also shifts. In C++ a mistake with pointers could crash the whole program. In TypeScript, most of my issues show up as type errors during compilation, or runtime exceptions if I misuse something. The safety net is there, but it forces me to think differently about what kinds of mistakes to expect.

These differences — especially the prototype-based inheritance chain — made me realize that learning TypeScript wasn’t just about picking up new syntax. It meant breaking away from my C++ mindset and understanding a completely different way of sharing behavior between objects.

## Athletic Software Engineering and WODs: A Great Way to Prepare

Pivoting towards athletic software engineering and the idea of “workouts of the day” (WODs), I’ve found the fast pace to be a real challenge. It’s not a rhythm I’m fully comfortable with yet, and trying to keep up has been a struggle. That said, my experience with online assessments (OAs) and technical interviews has shown me the value of this kind of structure.  

If you’ve ever used LeetCode, you know it’s a powerful tool for preparing for interviews. But it’s not always easy to sit down and grind problems without direction — the goals can feel vague or ambiguous, and it’s easy to lose motivation. What I appreciate about athletic software engineering and the WOD format is that it gives focus and accountability. Each “workout” provides a clear, specific task, and over time the repetition builds skill and confidence, just like physical training.  

For me, this structure turns practice into something more purposeful. Instead of endless problem sets, it feels like progress I can measure and build on — preparation that actually gets me closer to succeeding in interviews and, hopefully, breaking into the industry.

## Seeing into the Future

Looking ahead, I can see how these experiences fit together. Moving from C and C++ into TypeScript has pushed me to rethink how I approach programming, and learning OOP in a prototype-based world has stretched the way I think about design. At the same time, the structure of athletic software engineering and WODs has given me a framework for steady practice and growth, the same way athletes train day after day to get stronger. 

Even if my long-term focus is more on AI and machine learning, these lessons are still essential. Strong foundations in OOP and software engineering practices make it easier to build and maintain real systems, not just models in isolation. The discipline of consistent “workouts” builds habits I’ll carry into any technical challenge.  

I know getting into the industry is hard, but I can already feel how each small step — learning OOP, tackling WODs, staying consistent — is making me more prepared for the challenges ahead.
