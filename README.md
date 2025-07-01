# Guts

GPU Understanding Through Slogging (Guts) is a personal repository for studying GPU programming, or more specifically massive SIMD programming, step by step

## Principles

To push the study progressively, I decided to follow some principles
* For ways of SIMD, SIMD instruction sets are quite common in many platforms. But, too common. Even for x86 ones, I won't be happy for being lost among so many instruction sets from Intel and AMD. GPU is fine
* For programming languages, I decided to choose **C**, which is simple and straightforward. Those **object-oriented** ones are too complicated for dumb guys like me, and **functional** ones do not have good enough API support (it's a pity)
* After fixing the language, the choices of platforms are narrowed. **CUDA Driver API** may be the only playground for me. Alternatives such as ROCm and Ascend C only welcome C++ programmers
* The basic reference resources come from the course [CMPS 224/396AA - GPU Computing, AUB](https://www.youtube.com/playlist?list=PLZrjSW9GrEZE07f8gLECc0tfJwNDm75RW) in spring 2021, for the famous book **Programming Massively Parallel Processors: A Hands-on Approach**. The content is quite solid and quite suitable for self-studying. I can find the examples in the book everywhere in many real world applications. Also some topics I read from Internet will be included
* To maintain a consistent progress, I follow the [FreeBSD style(9)](https://man.freebsd.org/cgi/man.cgi?style(9))
* To keep everything simple, major tools used will be `nvcc`, `clang` and `make`. I will try to keep this set small enough, get rid of unnecessary ones if possible
* Describe the structure of this repository
  - The **Table of Contents** below will list linkings to the corresponding markdown files in sub-directories
  - Each sub-directory contains one markdown file as the document for that topic (chapter, example, project, etc., whatever), as well as corresponding makefile and source codes. I will try to make sub-directory stand-alone
* Since the license is **WTFPL**, I will drop the copyright comment in every source code file
* Wish I can finish this project, as the project name shows

## Table of Contents
