---
layout: default
title: Troubleshooting
description: This page is meant to explain how to solve common issues when installing or using KAMI Blue. 
---

## Troubleshooting

#### If you experience an issue and it's not listed here, please [open a new issue]({{ site.github.repository_url }}/issues/new/choose) and a contributor will help you further.

## Setup
#### Could not find tools.jar
If you encounter this error when building, you most likely don't have the Java Development Kit (JDK) installed.
Head over to [here](https://www.oracle.com/ca-en/java/technologies/javase/javase-jdk8-downloads.html) to download the Oracle JDK. Install it and try again.

#### Crashes before game starts with some obscure Java error
Set your application configuration's JRE in Intellij to a manual path to a downloaded and extracted *Oracle* Java 8 JRE

#### Crashes before game starts with SpongePowered error
Make sure your workspace is clean and run
./gradlew clean
./gradlew setupDecompWorkspace
./gradlew build

#### Minecraft not loading at all

Note: only applicable if running through Forge and not an IDE. 

What `.jar` are you using in your `mods` folder? Make sure to use the one that ends with `-release` (`VERSION-release.jar`)

#### Just doesn't work when using runClient
Don't use that, try running it through your IDE or building and running Forge normally

## When using Intellij / Eclipse

#### Crashes in game but it worked fine / errors link to files you haven't changed

Delete your `.gradle` cache
