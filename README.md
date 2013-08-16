# HiCursorWords MOD #

----------

## About ##

This script highlights words under the cursor like many IDEs.

This doesn't provide scope-aware highlighting nor language specific one.
You can control highlighting by highlighting group names. 

this is forked from [#4306](http://www.vim.org/scripts/script.php?script_id=4306 "http://www.vim.org/scripts/script.php?script_id=4306") by [Shuhei Kubota](http://www.vim.org/account/profile.php?user_id=7032 "Shuhei Kubota") and made a little change by 
[荒野无灯](http://ihacklog.com "荒野无灯@iHacklog")

HiCursorWords : Highlights words under the cursor. 

没错，这就是你要找的vim **高亮与当前光标下单词相同的所有单词** 的功能。

the original plugin set highlight group to **Underline**,I changed it to **MatchParen**

## Configuration ##

**highlight group:**

hicursorwords.vim line 49:

	highlight! link WordUnderTheCursor MatchParen

You can change it to what you want.


**default config:**
	
	let g:HiCursorWords_delay = 200
	let g:HiCursorWords_hiGroupRegexp = ''
	let g:HiCursorWords_debugEchoHiName = 0

**Variables explanation:**

(A right hand side value is a default value.)

	g:HiCursorWords_delay = 200

A delay for highlighting in milliseconds.
Smaller value may cause your machine slow down.

 	g:HiCursorWords_hiGroupRegexp = ''
If empty, all words are highlighted.
If not empty, only the specified highlight group is highlighted.
(my memo: 'Identifier\|vimOperParen')

To investigate highlight group name, the next variable may help you.

	g:HiCursorWords_debugEchoHiName = 0
If not 0, echoes the highlight group name under the cursor. 


## Installation details ##
Just put this file into the **plugin** directory. 


----------

That's all. Have fun `/*_*/`