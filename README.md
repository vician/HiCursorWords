# HiCursorWords MOD #

## About ##
this is forked from [#4306](http://www.vim.org/scripts/script.php?script_id=4306 "http://www.vim.org/scripts/script.php?script_id=4306") by [Shuhei Kubota](http://www.vim.org/account/profile.php?user_id=7032 "Shuhei Kubota") and made a little change by 
[荒野无灯](http://ihacklog.com "荒野无灯@iHacklog")

HiCursorWords : Highlights words under the cursor. 

没错，这就是你要找的vim**高亮与当前光标下单词相同的所有单词**的功能。

the original plugin set highlight group to **Underline**,I changed it to **MatchParen**

hicursorwords.vim line 49:

	highlight! link WordUnderTheCursor MatchParen

You can change it to what you want.

## Configuration ##

default config:
	
	let g:HiCursorWords_delay = 200
	let g:HiCursorWords_hiGroupRegexp = ''
	let g:HiCursorWords_debugEchoHiName = 0

That's all. Have fun `/*_*/`