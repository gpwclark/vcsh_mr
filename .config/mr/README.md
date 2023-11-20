1. Clone this repo

- mr gitGUIDE 1: http://www.linuxjournal.com/content/manage-your-configs-vcsh?page=0,2

- GUIDE 2: https://web.archive.org/web/20151009043051/http://www.geoffcorey.com/2015/03/managing-dotfiles-across-multiple-platforms/
- initializing a vcsh repo
	-  vcsh init <proj>
- adding stuff to extant vcsh repo
	-     vcsh enter vim
	- git add <the_file> # e.g. .vimrc
	- git commit -m "<a_comment>"
	- git push origin master
	- exit

    ! don't forget about `vcsh foreach add -u` and ``vcsh foreach status -uno` # to ignore untracked files

- settuing up a new machine
1. install mr and vcsh
2. 
```
vcsh clone git@github.com:gpwclark/vcsh_mr.git
```
3. Edit any desired configuration in .mrconfig file and the config directory in ~/.config/mr/
```
mr up
```
4. done!
