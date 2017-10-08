## vim

- <https://github.com/chriskempson/base16-vim/blob/master/colors/base16-default-light.vim> `c1c3e6c`
- <https://github.com/chriskempson/base16-vim/blob/master/colors/base16-default-dark.vim> `c1c3e6c`

```
3,10d | 4d | 5d | 36d | 42,49d |
4s#.*/#execute "silent !/bin/sh $HOME/.nightshell/# |
4s/\.sh// |
%s/base16-default/nemo/ |

%s/181818/0f141f/ |
%s/282828/182030/ |
%s/383838/293652/ |
%s/585858/384b70/ |
%s/b8b8b8/596e99/ |
%s/d8d8d8/8f9fbf/ |
%s/e8e8e8/c1cee8/ |
%s/f8f8f8/ebf1ff/ |

%s/ab4642/bf5062/ |
%s/dc9656/d47546/ |
%s/f7ca88/d4b000/ |
%s/a1b56c/609456/ |
%s/86c1b9/3e9486/ |
%s/7cafc2/6393ab/ |
%s/ba8baf/8572ab/ |
%s/a16946/ab7298/ |

%s/Character",    s:gui08, "", s:cterm08/Character",    s:gui0A, "", s:cterm0A/ |
%s/Cursor",        s:gui00, s:gui05, s:cterm00, s:cterm05/Cursor",        s:gui00, s:gui0A, s:cterm00, s:cterm0A/ |
%s/Identifier",   s:gui08, "", s:cterm08, "", "none/Identifier",   s:gui0A, "", s:cterm0A, "", "bold/ |
%s/LineNr",        s:gui03, s:gui01, s:cterm03/LineNr",        s:gui04, s:gui01, s:cterm04/ |
%s/Search",        s:gui03, s:gui0A, s:cterm03, s:cterm0A,  "", "")/Search",        s:gui00, s:gui0A, s:cterm00, s:cterm0A,  "", "")/ |
%s/statusline",    s:gui04, s:gui02, s:cterm04, s:cterm02/statusline",    s:gui05, s:gui0A, s:cterm05, s:cterm0A/ |
%s/StatusLineNC",  s:gui03, s:gui01, s:cterm03, s:cterm01/StatusLineNC",  s:gui05, s:gui01, s:cterm05, s:cterm01/ |
%s/Visual",        "", s:gui02, "", s:cterm02/Visual",        s:gui06, s:gui02, s:cterm06, s:cterm02/ |
%s/VisualNOS",     s:gui08, "", s:cterm08, "", ""/VisualNOS",     "", s:gui01, "", s:cterm01, "none"/ |
%s/WildMenu",      s:gui08, s:gui0A, s:cterm08, ""/WildMenu",      s:gui00, s:gui06, s:cterm00, s:cterm06/ |

if @% =~ 'dark' | 127s/05/02/g | 144s/03/04/g | endif |

normal =gg
```

## nightshell

- <https://raw.githubusercontent.com/chriskempson/base16-shell/master/scripts/base16-default-light.sh> `376294b`
- <https://raw.githubusercontent.com/chriskempson/base16-shell/master/scripts/base16-default-dark.sh> `376294b`

```
2,4d |

%s#18/18/18#1f/1f/1f# |
%s#28/28/28#36/36/36# |
%s#38/38/38#54/52/4d# |
%s#58/58/58#75/72/6c# |
%s#b8/b8/b8#94/90/88# |
%s#d8/d8/d8#ba/b5/ab# |
%s#e8/e8/e8#e0/da/ce# |
%s#f8/f8/f8#ff/f8/eb# |
%s#ab/46/42#bf/50/62# |
%s#dc/96/56#d4/75/46# |
%s#f7/ca/88#ab/98/2b# |
%s#a1/b5/6c#60/94/56# |
%s#86/c1/b9#3e/94/86# |
%s#7c/af/c2#63/93/ab# |
%s#ba/8b/af#85/72/ab# |
%s#a1/69/46#ab/72/98# |

%s/181818/1f1f1f/ge |
%s/383838/54524d/g |
%s/d8d8d8/bab5ab/g |
%s/f8f8f8/fff8eb/ge |

call append(123,["",
"echo -ne '\\e]12;#d47546\\a'"])
```
