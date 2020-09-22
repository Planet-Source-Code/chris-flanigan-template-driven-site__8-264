<div align="center">

## Template Driven Site


</div>

### Description

This code allows for the use of a template system on your website. You edit the code and specify the events that it should check and then you're all set. The code will take care of the document inclusions.
 
### More Info
 
You should know the 'pwd' of your home directory. You just tell it what documents to include...and it'll include it wherever you put the code.

Make your links < a href="?do=xxxx">whatever</a> where xxxx is the event corresponding to the code in your page.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Chris Flanigan](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/chris-flanigan.md)
**Level**          |Beginner
**User Rating**    |3.7 (11 globes from 3 users)
**Compatibility**  |PHP 3\.0, PHP 4\.0
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__8-1.md)
**World**          |[PHP](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/php.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/chris-flanigan-template-driven-site__8-264/archive/master.zip)

### API Declarations

Chris Flanigan


### Source Code

```
<?php
# ChrisF.net menu code. Edit at your discretion.
# No guarantees to the usefullness of this code is provided.
# http://whatever.com/?do=xxxxxxxx
# case "xxxxxxxx" compares the value of do and executes code
# accordingly
# Simply adjust each line according to what value you wish to compare # to
# Paste this code where you want the inclusion to take place
switch ($do) {
	# If $do = the following
    case "programming":
	# Perform this command
    include "programming.inc";
	# Keep the next line or you'll regret it >:)
    break;
  case "home":
	include "/home/chrisf/html/news.txt";
    break;
  case "tetrinet":
	 include "tetrinet.inc";
    break;
  case "computers":
	include "computers.inc";
    break;
  case "links":
	include "links.inc";
    break;
  case "friends";
	include "friends.inc";
	break;
  default:
	include "/home/chrisf/html/news.txt";
	break;
} ?>
```

