# Pythagorean Triples

## 🗝️ What is it?

This is a program that generates [Pythagorean triples](https://en.wikipedia.org/wiki/Pythagorean_triple) and uses them in a basic cryptosystem.

It does this by using [Racket](https://en.wikipedia.org/wiki/Racket_(programming_language)), a programming language whose use in said context shows mastery of functional programming paradigm and concepts.

The project is split in 4 parts, `etapa1` - `etapa4`, that I have worked on for a few couple of weeks during March 2022, and it's one of my favourite projects so far.

## ⚙️ How to run it?

1.  Clone this repository.
2.  Run the automated tests by opening the `checker.rkt` files using [DrRacket](https://download.racket-lang.org) and running them.
3.  Enjoy!

## 📐 What does it do?

The central idea of the program is that you can generate an infinite amount of Pythagorean triples by starting with the well-known triple `(3, 4, 5)` and multiplying it with a list of three matrices called `T1`, `T2` and `T3`.

Depending on the order of said three matrices in the list, one can get a unique Pythagorean triple. The entire process is explained further inside `etapa1/ppt.rkt`.

![image](https://user-images.githubusercontent.com/74200913/223983346-11de5feb-3d39-4bdf-b8ac-fa65c93207b2.png)

This process, even though it can be perceived as too math-intensive for the average user, can have very interesting uses in cryptography and Internet security. And this is exactly where the interesting stuff comes in.

By knowing about this simple yet elegant mechanism, two people communicating through a network can design a [symmetric-key algorithm](https://en.wikipedia.org/wiki/Symmetric-key_algorithm) to encrypt their messages.

For example, one can send a number `n`, that represents the nth Pythagorean triple in the triples tree, and use it to generate a key used to encrypt a text message. This way, the person receiving the message will use the number `n` to generate the key so they can decrypt it.

This process, a bit more complicated than what I described, is further explained in `etapa3/cryptosystem.rkt`.

## 🎡 Was it fun?

It was **incredibly** fun. Back then, I had 0 knowledge on functional programming and the way it can be different from mainstream, procedural programming.

So, learning to write something like this from scratch was very challenging, and it honestly felt like being back to square one and learning the basics of how to code all over again.

This is why it was an amazing experience: I would constantly not know how to proceed and lose sleep over one of those functions, only to wake up and feel extraordinary from having figured it out overnight.

## 🤔 Did you know?

Functional programming is very useful and complex, but if you don't know much about it you could remember the word "functional". It does use a lot of functions: for this simple program alone, I must have written around 54 functions alone. 🤓
