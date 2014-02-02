---
layout: post
title:  "Mac OS X command files"
date:   2014-01-19 17:20:00
categories: macosx command
---

I wanted a simple way to start and stop MySQL on my Mac laptop without having to go the command line and run <code>mysql.server start</code> all the time.

I found .command files.  They are basically shell scripts starting with !#/bin/sh that you make executable and name ending in .command.  Make a file with the contents of your script, then save it with a name like startmysql.command

<code>!#/bin/sh<br \>/usr/local/bin/mysql.server start</code>

Using <b>Open with</b> in the <b>Get Info</b> command you can tell Mac OS X to run the .command file within your favorite terminal program.

Now you have a file to start or stop your mysql server without typing the command each time.
