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

### adding items###

`things add` or `things new`: opens the quick entry panel

` things add new todo item`: adds a new item named `new todo item` to the Inbox

`things listname add new todo item`: adds a new item named `new todo item` to the list, area or project named `listname`

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










things check “todo”

marks the first item whose name starts with “todo” in the “Today” list as completed


things delete “todo”

deletes the first  item whose name starts with “todo” in the Today list


