---
title: Lightweight dependency injection in Elixir without the tears
categories: small
summary: Dependency injection is a tool to allow the runtime to pass dependencies into a function. This can be used to swap out implementations based on data being handled, or as a way to provide a mock implementation for testing.

article:
  title: Lightweight dependency injection in Elixir (without the tears)
  author: Andrew Hao
  twitter: andrewhao
  link: https://blog.carbonfive.com/2018/03/19/lightweight-dependency-injection-in-elixir-without-the-tears/
  archive: https://web.archive.org/web/20190920020949/https://blog.carbonfive.com/2018/03/19/lightweight-dependency-injection-in-elixir-without-the-tears/

tags:
  - elixir
  - dependency injection
  - code design
---

In _{{ page.article.title }}_, Andrew Hao goes in depth into how to perform four variations of dependency injection using Elixir.

After reviewing and thinking about the methods discussed, I find I am partial to _Approach 4: Protocols and data_.

Approach 4 uses protocols and structs[^1] to achieve a type-like way of defining functions. It is a little cumbersome due to having to define the type as a Struct, which is passed as the first parameter of the function being called. Once you wrap your head around it, it is a reasonable approach.

[^1]: [protocols and structs](https://elixir-lang.org/getting-started/protocols.html)
