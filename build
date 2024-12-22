#!/bin/zsh

# Check if an argument is provided
if [ -z "$1" ]; then
    echo "Usage: ./build.zsh <filename (without extension)>"
    exit 1
fi

# Force close the $file - PCB Editor window
wmctrl -c "$1 — PCB Editor"

# Build the project and open the PCB Editor
ergogen . && xdg-open ./output/pcbs/$1.kicad_pcb

return 0