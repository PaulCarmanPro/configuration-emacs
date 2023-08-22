# emacs-configuration

### Goal
Create a non-modal keyboard where every key functionally does the same thing all the time.

### Escape vs Ctrl-G
Emacs recognises the Escape key to be the early Meta key, which is sometimes emulated with AltGr, customairally Alt-Right. I can't say that I understand the Meta key which has evoloved out of existance. But, I do say that I like the Escape key to exit. Emacs calls the exit key Ctrl-G. Such knowlege is good, but I want Ctrl-G, being that it is next to Ctrl-F to be 'find again', or in practice, 'find next'.

- [ ] ESC should always to perform the action of Control-G. Current declarations are inadequate. There is no code which examines every keymap -- if Escape is undefined, then all keymaps should change the declaration under Control-G to Escape. I have a small measure of knowledge to such matters. Keymaps, is not a link list, can be stored in a complex manner. Emcas has a few basic prescidence levels. 

### More ToDo
- [ ] Crtl-PgUp/Dn changes from file to file. Consider replacing the function with TabBarMode.
- [ ] Ctrl-F/G does not work properly given a selected region.
- [ ] Cttl-A/E should  push cursor position, move to fisrt/last non-blank on line, move to bol/eol, move to bof/eof, select all, move to saved cursor postion and repeat.
- [ ] Ctrl-Y should not paste whole like unless whole line was yanked with Ctrl-K. Then, Ctrl-Y should become Ctrl-V. Ctrl-K should copy selected region if one exists. Result should be del|Ctrl-K/Ctrl-V easily replaces Copy/Cut/Paste because Crtl-C and Ctrl-X are primitively purposed. Currently, CuaMode is used.

### Comarison to Vim
Emacs and Vim are complete opposites. Loving speed, I initially chose to use Vim. I liked Vim, but I found the basic cursor movment keys which every macro must be built upon to be annoying. The very thing that gives Vim its speed, its immutable foundation, was clearly flawed and I didn't want to work with it. So I switched to Emacs. Emacs is incredibly huge and slow, but everything about it is mutable.

