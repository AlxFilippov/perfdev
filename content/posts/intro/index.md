+++
title = '!Performance ?'
date = 2026-01-03T07:07:07+01:00
draft = true
summary = 'Why do we even care about performance? It’s crucial to understand: it’s not just about "polishing" search algorithms or making sorting a bit faster.'
+++

# The Ultimate Goal

The ultimate goal is to deliver the product to the end-user as quickly as possible. But that raises a fair question: **"Faster than what?"** Is there a *golden number* or a specific metric we should aim for? Let’s break it down.

## First User Interaction

What does a user see first when interacting with your product?

- The app loading
- The splash screen
- The initial steps of the flow

Over time, app complexity grows, and the business tries to shove the un-shoveable into the tiny real estate of a smartphone screen. Displaying all of this requires more data and more processing power.

## Resource Competition

Some of that data can be offloaded to the background, but the real tug-of-war between product teams happens over the **"here and now."** Who gets rendered on the screen first? Everyone has conversion metrics to hit; everyone has to report to stakeholders. In essence, development turns into a literal battle for device resources.

And mobile resources are limited—both physically (hardware) and system-wide. Moreover, every year, mobile OSs tighten the screws, penalizing apps for excessive memory consumption or battery drain.

## Under the Hood

Let’s look a bit deeper under the hood. There is a fundamental law in mobile: **Don’t block the UI thread.** You only get one.

Но how do you handle it when a specific feature and its ten nested widgets needs to dump a massive pile of data on the user all at once, without lagging, and while keeping the user firmly in the sales funnel?

## The Practical Reality

You might say, *"Just don't block the thread,"* and you’d be absolutely right. We could call it a day right there. But in practice, this is where the **"hunger games"** begin: juggling asynchrony, parallelism, lazy loading, multi-level caching, and trying to mask it all with splash screens and shimmers.

## Process and Metrics

To keep the user’s path from **"click" to "business value"** unobstructed, you need to build processes and metrics around resource utilization across all teams working on the app.

## Performance as Balance

Performance is the art of balancing resource utilization. It’s a balancing act both internally (between components and teams) and externally (your app competing with the OS and other processes).

## The Numbers

Returning to the question of numbers: our primary North Stars are hard system constraints. In example **Frame timing (FPS)** and **battery consumption**. These metrics are only the entry point into the rabbit hole of performance.

Intro's over. Hope you didn't wander off to scroll through Reels.
