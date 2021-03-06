# Roku Ruby CLI Remote

Use a terminal and vi-like key bindings to control a Roku TV or device on your local network.

Built with ruby, curses, ssdp, and the Roku External Control API.

![Preview Vim Roku](https://giant.gfycat.com/UnfoldedSilkyDiscus.gif)

## Install / Usage
```
$ gem install roku-ruby
$ roku-remote
``````


## Key bindings:
```
        i                 info
        h                 left arrow
        j                 down arrow
        l                 right arrow
        k                 up arrow
        /                 search
        p                 power on
        enter             select
        escape            home screen (or cancel vi movement)
        del               back
        0..n              repeat next command N times
        escape (after n)  cancel N command
        -                 volume down
        =                 volume up
```

## caveats / todo
- only works with the first Roku device it finds on your network.. I only have one device to tests against, unsure what happens otherwise
- search functionality is implemented per Roku docs instructions, doesnt work though
- need a insert mode for text fields
- power off isn't documented.. -.-
- should highlight buttons on CLI screen when pressed
- should highlight numeric keys when N command activated

## other
- [Roku External Control API.](https://sdkdocs.roku.com/display/sdkdoc/External+Control+Guide)
- only tested on `ruby 2.3.1p112 (2016-04-26 revision 54768) [x86_64-darwin15]`. probably doesn't work on windows from what I read.

