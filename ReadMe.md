#ThingsCLITool#

Command line tool for [Things GTD app](http://culturedcode.com/things) by CulturedCode

## usage ##

```
things [list, area or project name] [help|open|show] [add|check|uncheck|cancel|delete|today|next|defer itemname]
```

## commands ##

### listing items###

` things `: lists the items in “Today”

`things listname`: list the items in the list, area or project named `listname`

`things show` or `things open`: open the "Today" view in Things

`things listname show`: show the list, area or project named `listname` in Things

###list output###
The result of a things command will look like this:

```
> things 'Things CLI Tool'
Things: project Things CLI Tool
*√ flag item as Today
 √ uncheck an item
 √ add an item
 √ check an item
 √ cancel an item
 √ delete an item
 - tag an item
 - read tags of an item
*- upload to github
```

The first line is show the name of the list, area or project the command was working on.

Then the tool will list the items. Completed items have a `√` and open (not completed) items have a `-`. Canceled items have an `x`.

Items marked for 'Today' will also have an asterisk `*`.

### adding items###

`things add` or `things new`: opens the quick entry panel

` things add todo item`: adds a new item named `todo item` to the Inbox

`things listname add todo item`: adds a new item named `todo item` to the list, area or project named `listname`

### checking items###

`things check someitem`: checks the first item in the "Today" list whose name starts with `someitem`

`things uncheck someitem`: unchecks the first item in the "Today" list whose name starts with `someitem`

`things cancel someitem`: cancels the first item in the "Today" list whose name starts with `someitem`

`things listname check someitem`: checks the first item in the list, area or project named `listname` whose name starts with `someitem`

`things listname uncheck someitem`: unchecks the first item in the list, area or project named `listname` whose name starts with `someitem`

`things listname cancel someitem`: cancels the first item in the list, area or project named `listname` whose name starts with `someitem`


### more options###

`things listname today someitem`: marks the first item in the list, area or project named `listname` for 'Today'

`things next someitem` or `things defer someitem`: removes the first item in the 'Today' list whose name starts with `someitem` from the Today list (removes the golden star)

`things listname next someitem` or ` things listname defer someitem`: removes the first item in the list, area or project named `listname` whose name starts with `someitem` from the Today list (removes the golden star)

`things delete someitem`: deletes the first item in the "Today" list whose name starts with `someitem`

`things listname delete someitem`: deletes the first item in the liast, area or project named `listname` whose name starts with `someitem`

###other commands###

`things help`: shows usage

## installation##
The things script obviously requires the Things app to be setup and running. It will be happy anywhere in your `$PATH`, or alternatively you can clone the project anywhere and put a symlink in `/usr/local/bin` or elsewhere in your `$PATH`.

