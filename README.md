# omtask

`omtask` is an omnibox task manager for people that want to finish tasks, not organize them.

## Introduction

`omtask` is an implementation of [Steve Losh's command-line t](http://stevelosh.com/projects/t), as a Google Chrome Extension. It is accessed purely from the Omnibox (Chrome's address bar).

**Why Not "Omnitask"?**

Lots of Google results.

## Usage

Type `t` then `space` to enter omtask mode.

### Add a Task

To add a task, type the description after entering *omtask mode*:

    t Clean the apartment
    t Update HTML5 video players
    t Eat lunch

### List Your Tasks

To see your tasks, enter *omtask mode* and hit enter without typing anything:

    t 
    <in new tab>
    [3] Eat lunch
    [2] Update HTML5 video players
    [1] Clean the apartment

This will load a new tab with a simple html list of your Tasks and their IDs. The list automatically updates when you add or delete a task.

### Delete a Task

To remove a task from your list, type `t ID -d` or `t -d ID`:

    t 2 -d
    t 
    <in new tab>
    [3] Eat lunch
    [1] Clean the apartment

### Clearing All Tasks

If you'd like to remove all tasks and start the ID count from 0, type `t -clear`.