---
layout: post
title:  "Spit screen with tmux"
date:   2014-02-02 17:17:00
categories: linux tmux
---

![Split screen tmux](/assets/tmux.png)

I have been a long time <code>screen</code> user when connecting to remote machines that I don't want to lose work if the connection drops, but I just recently started using <code>tmux</code> and I've been won over by it's split screen feature.

To start tmux just run <code>tmux</code> and it will start and give you a nice status bar at the bottom.  You can list out your tmux sessions with the command <code>tmux ls</code>, and then reattach to your session with <code>tmux attach</code> and the session number.

By far my favorite use for tmux is split screen so I can view multiple process outputs on the same server without opening another ssh window.  tmux uses ctrl-b for it's commands.  <code>ctrl-b "</code> will split the window horizontally, and <code>ctrl-b %</code> will split the window vertically.

The <a href="http://www.openbsd.org/cgi-bin/man.cgi?query=tmux&sektion=1">tmux manual</a> has got to be one of the largest man pages ever, it can do much much more too.

