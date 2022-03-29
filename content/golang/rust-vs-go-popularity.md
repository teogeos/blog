---
title: "Rust vs Go - Which Is More Popular?"
date: "2020-05-06"
categories: 
  - "golang"
  - "rust"
---

Go and Rust are two of the hottest compiled programming languages, but which is more popular, Go or Rust?. I develop in Go full-time and love it, and I'm learning more about Rust recently - it's an exciting language. Let's explore some differences between the two and look at which is growing faster in the popularity polls.

## Popularity Stats

According to the StackOverflow [2019 surveys](https://insights.stackoverflow.com/survey/2019#technology-_-programming-scripting-and-markup-languages), Go is ahead in the polls when it comes to programming and markup languages.

![](/img/Screen-Shot-2020-05-05-at-8.07.37-PM-815x1024.png)

However, compare that to the previous year:

![](/img/Screen-Shot-2020-05-05-at-8.15.06-PM-880x1024.png)

Rust **wasn't even on the chart** just one year before.

Go did grow by an impressive 1.6%, but it would seem Rust might be growing even faster as a percentage over time.

Some more supporting evidence for the hypothesis that Rust is growing faster is another poll - [the most loved languages survey](https://insights.stackoverflow.com/survey/2019#technology-_-most-loved-dreaded-and-wanted-languages):

![](/img/Screen-Shot-2020-05-05-at-8.18.40-PM-747x1024.png)

Rust is a clear leader here, but Go isn't far behind. There is a lot of hype around Rust right now, for good reason.

Let's take a look at the most dreaded languages:

![](/img/Screen-Shot-2020-05-05-at-8.19.08-PM-725x1024.png)

No one dreads Rust. I suspect that a contributing factor is that Rust isn't used much yet. That said, the data indicates that Rust is currently more loved and less dreaded. Hard to argue with that.

Go actually makes the most dreaded chart, but close to the bottom. I suspect most of the hate is salty Java devs that have been forced to move to Go and give up their precious objects. They had to give up generics as well up until now, but we'll have [generics in Go](https://qvault.io/golang/how-to-use-golangs-generics/) in 1.18.

## So Which Is Better?

I don't think one is strictly better than the other, and a lot comes down to preference. Let's examine the claims made by the maintainers:

![](/img/Golang-1024x578.png)

> Go is an open-source programming language that makes it easy to build simple, reliable, and efficient software.
> 
> [golang.org](https://golang.org/)

![](/img/rust-social.jpg)

> A language empowering everyone to build reliable and efficient software.
> 
> [rust-lang.org](https://www.rust-lang.org/)

Based on their official headlines it would seem they are in direct competition. The key difference is that Go also aims to be **simple**. Rust makes no such claim.

Here are my current fast and loose opinions on the strengths and weaknesses of each:

<table><tbody><tr><td></td><td>Go</td><td>Rust</td></tr><tr><td>Speed</td><td>✅✅</td><td>✅✅✅</td></tr><tr><td>Memory Safe</td><td>✅✅✅</td><td>✅✅✅</td></tr><tr><td>Simple</td><td>✅✅✅</td><td>✅</td></tr><tr><td>Standard Library</td><td>✅✅✅</td><td>✅✅</td></tr><tr><td>Memory Optimized</td><td>✅✅</td><td>✅✅✅</td></tr><tr><td>Support/Community</td><td>✅✅</td><td>✅</td></tr><tr><td>Concurrency (Simplicity)</td><td>✅✅✅</td><td>✅</td></tr></tbody></table>

Lane's Sloppy Rust vs Go Comparison

I think **Go will likely be the go-to for performant backend systems**. Go's rich standard library and easy concurrency makes standing up HTTP servers or other networked services simple and easy. Go is also faster, safer, and less memory intensive than most of the legacy competition. For example, Go is less memory intensive than Java and C#, faster than Python and Ruby, safer than C++.

Rust seems like it may steal some of the spotlights from Go in **deeper backend processes** that need to get every ounce of efficiency that they can from the hardware. In microservices and polyglot architectures, it makes sense to mix and match technologies behind the scenes a bit.

Even more important than web programming for Rust, I see it being used for more **systems-level applications**. Rust could easily steal some business from C and C++ for uses in embedded devices, command-line utilities, and so forth.

## Related Reading

- [Running Go in the Browser With Web Assembly (WASM)](https://qvault.io/2020/07/01/running-go-in-the-browser-with-web-assembly-wasm/)
- [Qvault Classroom Launches Golang Crash Course](https://qvault.io/2020/07/02/qvault-classroom-launches-golang-crash-course/)
- [Sorting in Go - Don't Reinvent This Wheel](https://qvault.io/2020/05/27/sorting-in-go-dont-reinvent-this-wheel/)