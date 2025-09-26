---
layout: essay
type: essay
title: "Linting My Way Forward"
date: 2025-09-25
published: true
labels:
  - Coding Standards
  - Collaborative Tools
---

<img width="200px" class="rounded float-start pe-4" src="../img/codingstandards/eslint.png">

Coming from a computer engineering background, I’ve always felt pretty comfortable writing code in C. In that environment, coding standards like indentation or formatting never seemed like a big deal to me. As long as there was some effort made to keep things consistent, the code was still perfectly readable. Maybe that’s because of the strict typing in C, or maybe it’s just that there are fewer ways to “stylize” code in the first place. A missing space here or an oddly indented block there doesn’t usually make the difference between understanding the logic or not.

That mindset shifted once I started working in TypeScript and using ESLint inside VSCode. Suddenly, I could see why coding standards were more than just “style police.” In a language with so much more going on — asynchronous functions, classes, interfaces, generics, callbacks, and especially anonymous functions — readability can quickly get messy. With anonymous functions in particular, the way they’re formatted can make or break whether a block of code is easy to follow or a confusing wall of symbols. Without consistent rules to guide how these constructs are written, even small projects can turn into a nightmare to read and maintain.

## Why Coding Standards Matter

On my own, I’ve often felt like coding standards don’t make a huge difference. I can usually read through code just fine, even if the indentation is a little off or the braces aren’t lined up exactly the same way every time. But things change completely when you’re working in a collaborative project that uses version control tools like Git.

The problem is that version control doesn’t judge code based on “human readability” — it just compares files line by line. That means two files can be functionally identical, but if one developer uses tabs while another uses spaces, or if one indents differently than the other, Git will mark them as totally different. When you go to merge branches on GitHub, the diff tool will scream at you with hundreds of line changes, even though nothing about the logic of the program actually changed.

I’ve personally run into this during group projects, and it’s incredibly frustrating. You see a commit or pull request that looks like it’s “changing” half the codebase, when in reality it’s just formatting differences. It wastes time, makes reviews harder, and clutters the project history. It’s in these moments that the value of coding standards becomes crystal clear — they prevent version control tools from turning small inconsistencies into massive, misleading changes.

## ESLint in Practice

Even though we haven’t done collaborative projects yet in ICS 314, I can already see where ESLint will shine. Once we start working in teams, having consistent standards enforced automatically will save us from painful Git diffs and endless merge headaches. Just knowing that everyone’s code will be formatted the same way means version control tools won’t flag unnecessary changes, and reading through pull requests will be far less painful.

In solo assignments, my experience with ESLint has been mostly positive. The tool is straightforward, and most of the formatting issues I run into are easy to fix. The quick-fix feature in VSCode makes it simple — one click and the errors are resolved. It keeps me from worrying too much about style so I can focus on the actual logic of my code.

That said, it hasn’t been completely frictionless. When I first installed ESLint, I ran into a problem that made me want to rip the keyboard out of my laptop and throw it across the room. Every time I saved a file, it would automatically reformat the entire thing to enforce coding standards. This might sound convenient, but it came with one huge issue: it kept converting all my single-quoted strings into double quotes, even though the ESLint rules required single quotes to pass error checks. The result was endless cycles of errors that I found massively frustrating. It took me quite a while to figure out how to fix that setting, and that was incredibly un-fun.

Overall, though, ESLint has been a helpful addition to my workflow. That early headache aside, it’s made writing code cleaner and more consistent — and I know that when I start working with others, its value will only grow.

## Moving Forward

Looking back, my perspective on coding standards has definitely shifted. When I was only working in languages like C and ARM Assembly, they never seemed that important. I could read code just fine even if the formatting wasn’t perfect, and small differences didn’t get in the way. But moving into TypeScript — and especially thinking about how version control systems handle formatting — I’ve come to see why standards matter. They aren’t just about style; they’re about making collaboration easier and preventing headaches before they happen.

My experience with ESLint so far has reflected that. On my own, it’s kept me writing cleaner, more consistent code, and even if it’s occasionally frustrating (I won’t forget the single vs. double quotes incident anytime soon), the benefits outweigh the annoyances. And once we start collaborative projects, I know those benefits will become even more obvious.

In the bigger picture, I see coding standards as part of the foundation I need to grow as a software engineer. Tools like ESLint help form good habits now, so that when the projects get larger and the teams get bigger, I’ll be ready to focus on solving problems instead of wasting time on formatting battles.
