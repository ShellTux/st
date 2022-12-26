# My ST build

This is my st build made possible by [bakkeby st-flexipatch](https://github.com/bakkeby/st-flexipatch),
and [flexipatch-finalizer](https://github.com/bakkeby/flexipatch-finalizer)

List of enabled patches:

- ALPHA_PATCH
- ALPHA_FOCUS_HIGHLIGHT_PATCH
- ANYSIZE_PATCH
- BLINKING_CURSOR_PATCH
- BOLD_IS_NOT_BRIGHT_PATCH
- BOXDRAW_PATCH
- COLUMNS_PATCH
- COPYURL_PATCH
- CSI_22_23_PATCH
- DEFAULT_CURSOR_PATCH
- DELKEY_PATCH
- DYNAMIC_CURSOR_COLOR_PATCH
- EXTERNALPIPE_PATCH
- FIXKEYBOARDINPUT_PATCH
- FONT2_PATCH
- FULLSCREEN_PATCH
- INVERT_PATCH
- ISO14755_PATCH
- LIGATURES_PATCH
- NETWMICON_PATCH
- NEWTERM_PATCH
- OPENURLONCLICK_PATCH
- SCROLLBACK_PATCH
- SCROLLBACK_MOUSE_PATCH
- SCROLLBACK_MOUSE_ALTSCREEN_PATCH
- SIXEL_PATCH
- THEMED_CURSOR_PATCH
- UNDERCURL_PATCH
- UNIVERSCROLL_PATCH
- WIDE_GLYPHS_PATCH
- WORKINGDIR_PATCH
- XRESOURCES_PATCH
- XRESOURCES_RELOAD_PATCH

st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.


Requirements
------------
In order to build st you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.
