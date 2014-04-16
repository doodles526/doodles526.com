---
title: "Day 1: Hugo"
date: "2014-04-12"
slug: "day1-hugo"
Tags: ["Hugo", "Web-dev", "projects"]
Topics: ["Projects"]
Section: "project-every-day"
---

My first day of working on projects every I set out to create my blog.
I knew I wanted to use a static site generator, and I knew for some reason
I never really cared to start learning about node.  So why not use an SSG
written in my favorite compiled language, golang!

I started with a couple Google searches and found Hugo, a very fast, powerful,
and feature heavy static site generator written in Go.  It had everything that
I wanted, plus a lot more that I realized I might want later on.  The main
features that drew me in was that it wasn't blog-centric, easily installed, it was fast (~1ms per element),
automatic permalink structure, and automatic RSS creation.

With Hugo not being blog-centric, I can be assured that I can implement other static
sites without having to re-learn another SSG.  I would rather devote my time to making
Flask or Django apps than floundering for a few hours orienting with a new SSG.

To be honest I found the "minimal" example to be a bit complicated for learning, while
it is very complete.  Luckily, spf13 made his own blog using Hugo which is much more
minimal and serves as quite an excellent getting started tutorial.

Now that I've given a proper introduction to Hugo, I would like to give a brief overview of
setup and my work for the day.

I already had Go installed, so getting hugo was as easy as:
	go get github.com/spf13/hugo

After this I needed to setup a simple file structure:

>	./
>		./config.yaml
>		./content
>			./post
>			./project-every-day
>		./layouts