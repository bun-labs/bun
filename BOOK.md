# Bun Book

# Download 2 stage
Go to https://github.com/bun-labs/bun/releases
and download the latest release

# Setting up Loader
Go to the Bun releases page and download `loader.zip`.
Extract the archive and open `geometry.load`.
Locate `SYSNAME` and change it to `Bun` (optional).
Set `VER` to `bun`.
Find `baseinit()` and replace its contents with the following:
tput cnorm
[ -f /bun/kernel/bunkrnl ] && /bun/kernel/bunkrnl && exit 0
}
Create a directory named `fs/geo`.
Place the `geometry.load` file into `fs/geo/`.
