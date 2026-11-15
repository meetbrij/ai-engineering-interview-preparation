# Preface

> **Draft.** This is a starting point written for me to edit. Placeholders are in [square brackets].

## Why this exists

I have spent [N] years as a software engineer building and running production systems. When I decided to move into AI engineering, I found plenty of material, but it was scattered: vendor blogs, papers, courses, short videos, and interview question lists that disagreed with each other and sometimes got basic facts wrong. I wanted one place that explained the concepts in plain English, in the order you need them, and that showed how the pieces fit together in a real system.

So I started writing it down. This handbook is the result so far. It is my study notes, organised as a book, and it is meant to keep changing.

## Who it is for

It is written for **software engineers moving into AI engineering**, including forward deployed engineer and AI solution architect roles. It assumes you are comfortable with APIs, databases, cloud services and the basics of distributed systems. You do not need a machine learning background, because Parts 1 and 2 build the foundations.

It is not aimed at complete beginners to programming, or at people who want to do model research.

## How it was made

I want to be clear about this. **The text was drafted with an AI assistant (Claude, from Anthropic)**, working from an outline and a set of rules that I wrote, my own study notes, and public sources such as official documentation, papers and vendor engineering blogs. I am reading it, correcting it and extending it as I study. It has not had expert review, and it is not yet checked line by line.

Because of that, it can contain mistakes. Where a fact changes quickly (model names, prices, product features, regulations), it is marked "(as of Nov 2026)" and linked to a source. Where I could only find secondary sources, the text says so. Please check anything that matters before relying on it.

## How to read it

You do not need to read it from start to finish. Chapters are numbered in learning order, but each one is meant to stand on its own. A good way in is to read the "Key takeaways" at the end of a chapter, then go back to the parts you need.

The interview answers are written in the first person, as examples of how an answer can sound. They are not scripts. Adapt them to your own experience.

## What is deliberately left out

There is **no code** in the handbook. Interviews and design reviews test concepts and trade-offs, and code samples go out of date faster than ideas. Code is also better learned by building, which is what the companion project is for.

The chapter on privacy and regulation is **not legal advice**.

## What comes next

I plan to build an agent step by step, in public, one small change a day for about 30 days: a basic agent, then retrieval, tool calling, memory, evaluation, guardrails and so on. Each step will link back to the chapters here, so the handbook is the reference and the project is the practice. I also plan to turn some of the most useful chapters into shorter posts.

## Corrections and ideas

This is a living document. If you find an error, an outdated fact or a gap, please open an issue or a pull request with the chapter, what looks wrong and a source if you have one. Ideas are welcome too.

Thank you for reading.

[Your name]
[Date]
