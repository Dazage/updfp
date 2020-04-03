# updfp

My answer to flatpak applications not showing up in dmenu.

# Using

The script assumes that ~/.local/bin and all it's subdirectories are in your $PATH.

If that's not the case you can do so by adding the following to your ~/.profile:

`du $HOME/.local/bin/ | awk -F'\t' '{print $2}' | tr '\n' ':' | sed 's/:*$//'`

# Hacking

If you'd rather the launcher scripts go in a different location all you need to
do change the fp_scripts variable to the desired location.