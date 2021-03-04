---
layout: post
title: Wickedness
subtitle: part 2
tags: [minecraft, modding, VSCode, games, java]
comments: true
published: false
---

Welcome to part 2 of my Minecraft modding voyage!

As a preamble I want to say I'm not a IDE guy. I use VIM and a bit of Sublime Text in my Linux machines and sometimes in Windows too.
But I really like what the Microsoft team does with the Visual Studio Code IDE and I'm going to use it for Java and Minecraft modding.

1. Install the Java Extension Pack, which contains these popular extensions:
  - Language Support for Java(TM) by Red Hat  
  - Debugger for Java  
  - Java Test Runner  
  - Maven for Java  
  - Project Manager for Java  
  - Visual Studio IntelliCode  
2. Install the Gradle Extension Pack, Minecraft Essentials Extension Pack, and the Better TOML extention
3. Restart VSCode
4. Download 1.16.5 [Forge](http://files.minecraftforge.net/maven/net/minecraftforge/forge/index_1.16.5.html) and extract the 1.16.5-36.0.45/forge-1.16.5-36.0.45-mdk.zip file
5. Follow the instructions from the [Documentation](https://mcforge.readthedocs.io/en/1.15.x/gettingstarted/)  
 there's a VSCode specific task named `genVSCodeRuns` which can be run through the Gradle tab found on the left panel
6. Copy the `src` directory from the forge archive to our project main directory (overwriting it)
7. Modify the path to our mod Java class from `src\main\java\com\example\examplemod` to `src\main\java\com\vendor\modid`, in our case `com\kc00l\wickedness`
8. Modify `build.gradle` file:
  - replacing `modid` with `wickedness`
  - replacing `yourname` with `kc00l`
  - replacing `examplemod` with `wickedness`
  - replacing `examplemodsareus` with `kc00l`
9. Modify `src\main\resources\META-INF\mods.toml`
