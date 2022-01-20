# A script for polybar to display rofications.

## How to install

1. Copy bin/rofication-status to ~/bin, make sure ~/bin is in your $PATH. We don't want the styles in the output, just the number of notifications.
2. Copy the script in .config/polybar/scripts to ~/.config/polybar/scripts (or whatever location you prefer). 
3. Be sure to make both executable, and check that rofification-status gives the correct output (an integer).
4. Add this to your polybar config: 
    `[module/rofication-status]
    type = custom/script
    exec = ~/.config/polybar/scripts/rofication.sh
    click-left = ~/.config/polybar/scripts/rofication.sh --show &`
