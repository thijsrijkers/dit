# dit

**dit** is a small tool that lets you run scripts from your terminal with a single command, and knows which script to run based on where you are.

## The idea

You type `dit .` in any folder. Dit looks up whether you've told it what to do in that specific location, and if so, it runs that script. If not, it falls back to a generic script you've set up as a default. You get the right automation for the right context, without thinking about it.

When you just type `dit` with no arguments, you get an interactive menu in your terminal. From there you can create scripts, assign them to specific folders, and set your generic fallback. Everything is managed in one place.

## Why

Most automation tools are either global (they run the same thing everywhere) or project specific (they require a config file in every repo). Dit sits on your machine, no config files to commit, no setup per project.

The mental model is simple: every folder can have its own "what to do here" command, and if it doesn't, there's a sensible default waiting.

## How it feels to use

You're in a project folder. You type `dit .`. Your build script runs. You move to a notes folder. You type `dit .`. Your sync script runs. You go somewhere new. You type `dit .`. Dit tells you nothing is set up here, and reminds you how to fix that.

Over time, `dit .` becomes a habit, a single gesture that means *do the thing for this place*.
