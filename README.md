#### pkhakingvim

- cp3
{}, move to beginning of para, end of para  
(), move to beginning of sen, end of sen  
g, g;  move to previous changelist(s)  

[[ : move to next function
]]: move to pre function
[{: move to the beginning of the block
]}: move to the end of the block

gd: find where a var is defined

gk gj: can move up/down warpped line

- cp6 
vim scripting  
EX:  
```
:syntax match comments "/\*.*\*/"
:syntax keyword vars x y
:syntax match symbols "[{}();=]"
:syntax keyword keywords if return
:highlight vars ctermfg=red guifg=blue
:highlight symbols ........
:highlight comments
:highlight keywords
```

Region,can contains hilighted function syntax. using contains
```
:syntax region commentregion start="/\/\*/ end=/\*\// contains=keyword1,keywords2
```
