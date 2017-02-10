---
layout: essay
type: essay
title: Have Some Standards
date: 2017-02-09
labels:
  - ICS 314
  - Coding Standards
  - ESLint
---

## Coding Standard, what it is

According to this [Wikipedia article](https://en.wikipedia.org/wiki/Coding_conventions#Coding_standards) a coding standard is a set of rules for a programmer to follow when writing and formatting code meant to increase the quality of the source code.

Coding standards increase the readability of code; nice when your working on large projects, great when working with a team. Consistent indentation and spacing make understanding the code much faster.

### Efficiency and aesthetics not convincing enough?

When I started learning C I was told to declare all the variables at the beginning of the function, before writing any other lines of code. At first I thought it was just to make it easy to figure out what variables were available to the function. So when I wrote a function that needed error checking on the parameters I thought it would be fine to do the check first then define the variables. It worked using gcc as my compiler, but I also had to use Visual Studio. My code did not compile because variables were declared after other lines of code. Some rules in a coding standard have an even more practical purpose, ensuring that the code compiles with any compiler.

Then there is the AirBnB coding standard for JavaScript, which disallows the unary operators <code>++</code> and <code>--</code>. The [ESLint page](http://eslint.org/docs/rules/no-plusplus) explains that it is because these operators behave differently purely due to whitespace differences. Using the coding standard ensures that code behaves as expected.

## Enforce it

Having some rules are great, but there needs to be a way to ensure you and your team use them. Having someone on the team to proof-read the code to ensure that it follows the standard is not realistic, especially with several thousand lines of code. This is where a [lint](https://en.wikipedia.org/wiki/Lint_(software)) comes into play.

### ESLint with IntelliJ

The first lint I used is ESLint, made to flag coding standard errors in Javascript. Honestly, enabling it in IntelliJ was a bit of a pain; I would think I had enabled it, then realize I accidentally disabled it at some point. Then I found the AirBnB standard to be strict. However, it is easy to search for the error that ESLint is flagging and understand why it is an error and I find that having ESLint enabled makes it more tempting to follow the AirBnB standard since I would have to look at red lines throughout my code if I ignored it. It always runs so I can fix any mistakes as they occur. Overall I find having ESLint was worth the trouble of figuring out what I did wrong when trying to enable it.

<b>Now go get some standards!</b>