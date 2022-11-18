### My Build of sent:
Simple plaintext presentation tool cause pptx are just bloats and they suck.

### Applied Patches
- [Progress Bar](https://tools.suckless.org/sent/patches/progress-bar/): This patch introduces a progress bar at the very bottom of non-image slides. Similar to the slide numbers patch, it may be useful for an audience to know how much more of a presentation they have to endure. One way of measuring this is to add a bar to the slides which indicate the presenter's progress based on slide count.

- [Inverted Colors](https://tools.suckless.org/sent/patches/inverted-colors/): This patch adds another color scheme. You can switch to that alternate color scheme with the -i flag. You no longer need to recompile sent if you want to present with a different color scheme.

- [Toggle Colorscheme
](https://tools.suckless.org/sent/patches/toggle-scm/): This patch is meant to be applied on top of [inverted colors](https://tools.suckless.org/sent/patches/inverted-colors/). It adds a new binding, "i", which lets you toggle between the two colorschemes during presentation.

### Requirements/Dependencies
- libxft
- fontconfig
- libpng
- Comic Sans Ms font (If you want to use another font edit in the configuration)
- farbfeld (optional)

### Configuration and installation
Edit config.mk to match your local setup (sent is installed into the /usr/local namespace by default).

The configuration of sent is done copying [config.def.h](config.def.h) to `config.h`, editing it and then (re)compiling the source code.
