---
title: "From zero to 6502 assembly - how to teach yourself programming"
date: 2021-09-20T10:55:28+02:00
draft: false
thumbnail: /upload/2021/assembly.jpg
tags: ["assembly", "programming", "code", "6502", "6502 assembly", "demoscene"]
categories: ["Programming", "6502"]
sidebar: "right"
comments: true
---

**Assembly language**, this term alone raises mixed feelings. We admire programmers who write in low-level languages, and sometimes we see a bit of superhuman in them. Often, beginner (and even advanced) programmers are concerned about assembly languages. This also applies to me. I was never interested in programming 8-bit computers because I thought that BASIC was quite limited, and the 6502 assembly was a field completely beyond my intellectual abilities. I started to verify my view some time ago, when in one of his films, the famous YouTuber, The 8 Bit Guy, suggested that the opinion stating that the 6502 assembly belongs to extremely difficult languages is greatly exaggerated. Today, I think he was right - anyone can learn assembly language programming. How to go about it, where to start and what to do if you would like to create your own demos, and you do not have any programming experience? In this post, I will try to suggest solutions to people who would like to start programming.  
  
I have already put forward one thesis: anyone can learn assembly language. Another statement must be added - to learn to code, reading books and articles is not enough, **you have to implement your own projects**. I know far too many computer science graduates, people who have invested in bootcamps, who now cannot write code. This is because they took the time to memorize the syntax of the language, recreated the tutorials, but never took up the challenge on their own.  
  
The optimal way to independently learn programming is therefore learning based on the implementation of your own projects. We don't necessarily have to come up with groundbreaking things, nor do they have to be difficult programs. We can often draw inspiration from the available tutorials and create our own programs based on them, by expanding the topic and having our own idea.  
  
Immediately after learning the basics of any programming language, it is worth learning a library available for this language, it is best to choose a library dedicated to the things you want to do. Future demoscene authors may be interested in libraries dedicated to creating graphics and games.  
  
### Your first programming language
  
Interesting options: BASIC, Python, C.  
  
In the 1980s and 1990s, when 8-bit computers were present in the homes of enthusiasts, the first language of many demoscene makers was **BASIC**. Even today, it is a pretty good option to start with. In particular, if you treat programming as a hobby and do not dream of a career in the IT industry.  
There is (and is quite popular with retro computer enthusiasts) the Batari Basic project that allows you to program games for the Atari 2600 on a modern computer. There is no shortage of tutorials and enthusiasts who create their own libraries extending the possibilities of this language.  
  
**Pros of batari Basic**: the language is simple, you can learn it very quickly, and you can quickly create your first own game. Additional libraries are written in assembly language, so implementing the project in batari Basic will provide you with some contact with assembly.
  
**Cons of the batari Basic**: you will quickly feel the need to use something that will give you more options and allow you to go beyond the Atari 2600 
  
[Introduction to batari Basic](https://www.randomterrain.com/atari-2600-memories-batari-basic-commands.html) | [Kernel for creating high-quality titlescreens](https://atariage.com/forums/topic/169819-the-titlescreen-kernel/)
  
I can venture to say that today, **Python** is what BASIC used to be - a simple language for everyone. In addition, it has a huge number of libraries that allow for easy and quick creation of programs that perform almost any task. I started programming in Python a few years ago, I wrote and sold my first commercial program after a few days of learning, interestingly, thanks to the available libraries, my program only had 17 lines of code.  
  
**Pros of Python**: Python is a very beginner-friendly language, and writing a useful program can often be as simple as using the right library. One of the many libraries available for Python is [PyGame](https://www.pygame.org/) for graphics and game development. Python and PyGame are a quick start to gamedev. Due to the fact that it is a scripting language, your program will run on any modern computer (although in order to achieve this, the programmer needs to be aware of some basic aspects).  sidebar: "right"
comments: true
  
**Cons of Python**: aside from the fact that it allows you to learn programming, it's actually not very much related to the demoscene. It is a scripting language, which makes any program written in Python much slower than a compiled program (although it is possible to create executable binary files from Python code).  
  
[Programming in Python for beginners – the entire course in one video](https://www.youtube.com/watch?v=rfscVS0vtbw) | [PyGame for Beginners](https://www.youtube.com/watch?v=FfWpgLFMI7w)
  
**C** was my first programming language. They say it's a good idea to choose C as your first language. C is elegant, it is available on almost all machines - modern computers, retro computers, microcontrollers. C is demanding - writing advanced programs requires an understanding of how computer memory works, and the language is sometimes close to assembly. Many available libraries, courses and tutorials facilitate learning and once mastered C will allow you to create games and applications for both modern PCs and retro computers.  
  
**Pros of C**: The language is versatile, any knowledge of C will prove useful in the future, even if you quickly decide to move to another language. The Allegro library is available, a gamedev classic, which is a great tool for professional graphics and game programming. Thanks to the project [CC65](https://cc65.github.io/) you can program in C on your computer, thus creating programs that run on classic 8-bit computers.  
  
**Cons of C**: It is hard to master. To be a good C programmer, you need to understand the basics of a computer and the mathematical foundations of number systems. However, it is not very difficult and everything will turn out to be useful in assembly.  
  
[Learn C Programming Language basics in just a few hours](https://www.freecodecamp.org/news/the-c-beginners-handbook/) | [Quick tutorial for Allegro library](https://github.com/liballeg/allegro_wiki/wiki/Allegro-Vivace)  
  
### Let’s start with 6502 assembly
  
After you have mastered the basics of the language, familiarized yourself with the selected programming library and developed your own application or game, you can say that you know how to program. You can focus on what you can do and create new things in Batari Basic or PyGame or Allegro (or other languages and libraries). You may also be interested in 6502 assembly. Many popular 8-bit computers and consoles were equipped with a 6502 processor, so you will be faced with a choice - which machine exactly do you want to devote to?  
  
Luckily, you don't have to make that decision right away to learn the 6502 basics, and you don't even need to install any software. A free, [web browser-based interactive tutorial](https://skilldrick.github.io/easy6502/) is available.  
When starting your first assembly projects, it is necessary to understand numeral systems (decimal, binary, hexadecimal). You don't necessarily need to be fluent in converting and performing math, try to at least understand the essence of the issue because it's crucial.  
Sometimes, finding one good book can be the solution to a novice programmer's problems. I can recommend * Atari 130XE Machine Language for the Absolute Beginner * by Kevin Bergin, available for free to download from the website [atarimania.com](http://www.atarimania.com/documents-atari-400-800-xl-xe-books_1_8 .html). The book perfectly and in the accessible to beginners way explains the structure of 8-bit Atari, numeral systems and programming in the 6502 assembly.  
However, it should be noted that the programming tools proposed in the book are not any more the best choice. It is worth taking an interest in the compilers available today: [XASM](https://github.com/pfusik/xasm), [CA65](https://cc65.github.io/) - yes, ca65 is a part of cc65.  
  
This text does not describe all available languages, libraries or possibilities. It is only meant to inspire people who are looking for their way. If you can suggest other interesting tools or sources of knowledge - let me know in the comment. 