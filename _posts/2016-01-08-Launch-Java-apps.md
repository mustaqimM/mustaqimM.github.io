---
layout: post
title:  "Launch Java apps from the terminal"
date:   2016-11-20
desc: "Launch .jar"
keywords: "linux,windows,java,jar"
categories: [Linux,Windows]
tags: [Java,jar,shell]
icon: fa-lock
---

To launch a Java app, a .jar needs to be executed. A simple command would be ```java -jar JavaApp.jar```. You would also need to disown the
process from the terminal or the terminal would need to be left open. To do this, change to the directoy where the ```.jar``` is located; execute
```java -jar JavaApp.jar``` to /dev/null. The entire command would be something like:
```cd /JavaAppDirectory/; java -jar JavaApp.jar &!; exit 1"```

The ```&!``` command is a zsh-specific shortcut to send the app to the background and disown the process, so that exiting the shell will leave it running. It can be substituted for the bash equivalent bash ``` > /dev/null ```
