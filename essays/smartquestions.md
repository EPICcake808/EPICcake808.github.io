---
layout: essay
type: essay
title: "Questions That Teach vs. Questions That Drain"
date: 2025-09-11
published: true
labels:
  - Software Engineering
  - Typescript
---

<img width="200px" class="rounded float-start pe-4" src="../img/typescript/typescript.jpg">

## Stack Overflow Heaven vs. Reddit Swamp

One of the biggest things I’ve learned — not just in software engineering, but in life — is that *how* you ask a question matters just as much as the question itself. Whether it was homework back in school, troubleshooting some obscure PC problem, or now debugging code, I’ve seen the same pattern repeat over and over. If you ask vaguely, you usually get vague answers. But if you put effort into explaining the problem, half the time it feels like the solution reveals itself while you’re writing it out.  

Eric Raymond’s essay *How to Ask Questions the Smart Way* really drove that home for me. His guidelines can come off a little blunt, but they’re true: communities thrive when people put effort into their questions, and they suffer when people treat them like a free tech support hotline. I’ve noticed the same thing myself while browsing online spaces. Some places, like Reddit, are full of low-effort posts that could’ve been answered with a two-second Google search, and it drags the whole discussion down. StackOverflow, on the other hand, enforces stricter standards — and while that might seem harsh at first, it’s what keeps the quality of posts high.  

For this essay, I’ll be looking at two examples from StackOverflow: one where a developer asked the “smart way” and got a clear, efficient answer, and another where the opposite happened. Comparing them made me realize just how much asking questions the right way matters, not just for getting help, but for being part of the engineering community at all.

## A Smart Question on StackOverflow

A good example of the “smart way” comes from a [classic C question](https://stackoverflow.com/questions/605845/should-i-cast-the-result-of-malloc-in-c) about `malloc` . The developer asked why many C programmers recommend **not casting the result of `malloc`**. They showed two versions of the same line of code:

```c
int *sieve = malloc(sizeof(*sieve) * length);        // no cast
int *sieve = (int *) malloc(sizeof(*sieve) * length); // with cast
```

and then asked, “Why would this be the case?”

This hits almost every one of Eric Raymond’s guidelines. The question is minimal (only the two lines of code that matter), clear (C vs. C++ context), and precise (“Why is the first preferred?”). It doesn’t ask anyone to do the asker’s work for them, it just asks for clarification about a specific practice that seems confusing. Because the asker framed it so cleanly, the answers were high quality.

Multiple experts responded with thoughtful explanations:

"In C, casting the return value of malloc is unnecessary because malloc returns a void *, which automatically converts to any object pointer type."

"Casting can actually be dangerous in C because it hides errors. If you forget to #include <stdlib.h>, the compiler may assume malloc returns an int and silently convert it, leading to undefined behavior."

"The cast is only required in C++, which is where the confusion often comes from."

"The idiom sizeof *sieve is safer than sizeof(int) because it adapts automatically if the variable’s type changes."

The community converged quickly on the correct reasoning, with highly upvoted answers and citations to the C standard. This is a textbook case of Raymond’s principle that good questions are a gift: the asker framed a specific, thought-provoking question that prompted clear, educational answers not just for themselves, but for thousands of future readers who’ve had the same doubt.

## A Not-So-Smart Question on StackOverflow

To see the opposite case, imagine a post like this one (AI generated):

**Title:** *HELP! malloc doesn’t work!!!*  

**Body:**  
> Hi everyone, I’m trying to use malloc in C but my program keeps crashing. Can someone just fix it for me? Here’s my code:  
> 
> ```c
> int main() {
>   int *arr;
>   malloc(100);
>   arr[0] = 5;
> }
> ```  
> 
> Urgent!! Please help ASAP, my homework is due tonight!!!  

I’ve come across posts like this plenty of times, and they usually don’t go well. The title doesn’t explain the problem, and the body doesn’t show much effort beyond pasting a short code snippet. There’s no context about what the programmer expected to happen, what they tried to do to fix it, or even what error messages they got. On top of that, throwing in words like “urgent” or “important” tends to backfire — people on StackOverflow don’t feel inclined to solve your assignments for you.

Because of that, questions like this rarely get useful answers. Most of the time they get downvoted or closed, and any responses are short and blunt, pointing out obvious mistakes or telling the asker to check the manual. Compared to the earlier `malloc` question, which sparked detailed and thoughtful discussion, this one doesn’t teach much to anyone — not the person asking, and not the community reading. It’s a good reminder that the way you frame a question really does decide whether you get help or just frustration in return.

I've been in those shoes, needing help on a homework assignment due at 8 AM, and I understand that it is incredibly important when you need help on an assignment you don't understand. However, seeking help on online forums with questions worded like this won't get you those helpful answers quickly. As mentioned above, you're more likely to receive downvotes and scorn than anything else.

## Why I’d Rather Be on StackOverflow

Putting these two examples side by side really shows the difference. The first question about casting the result of `malloc` was short, clear, and to the point. It showed the exact code, asked a specific “why,” and left room for people to explain. Because of that, the answers were high-quality and actually useful, not just for the person asking but for anyone who stumbles across it later.  

The second example went the other way. A vague title, sloppy code, and an “urgent homework” vibe — that kind of thing almost never gets good answers. More often than not, it just ends with downvotes or blunt comments telling the asker to check the manual. I’ve seen posts like that plenty of times, and they don’t teach anyone much of anything.  

What I take away from this is that asking smart questions is really about making it easier for other people to help you. If you put in the effort up front — show what you tried, be clear, be specific — people are way more willing to meet you halfway. And when they do, the answers you get are usually way more valuable. That’s something I try to keep in mind not just online, but any time I’m asking for help.  

I notice this difference the most when I compare StackOverflow to Reddit. On Reddit’s technical subreddits, I constantly see low-effort questions — things that could be answered with a quick search or even an AI tool. It gets draining, because it pushes the real technical conversations further down. StackOverflow is far from perfect, but its higher standards make the whole experience better. Even if it feels harsh at times, I’d rather be in a community where the expectation is that you show effort and respect the time of the people trying to help you.  
