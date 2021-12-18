# ani-cli for MacOS

This is a fork of the original [ani-cli](https://github.com/pystardust/ani-cli).
This fork intended to support macOS on the go and a full instalation guide.

This tool scrapes the site [gogoanime](https://gogoanime.pe).

## Download

Download homebrew
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Download mpv
```bash
brew install --cask mpv
```

Cloning repo. Make sure its in your desired directory
```bash
git clone https://github.com/Hanndot/ani-cli-macos.git
```

## Install

Change directory to the project directory
```bash
cd ani-cli-macos
```

Install using Makefile
```bash
sudo make
```

## Usage

  ### watch anime
  ``ani-cli <query>``

  ### download anime
  ``ani-cli -d <query>``

  ### resume watching anime
  ``ani-cli -H``

  ### delete anime from history
  ``ani-cli -D``

  ### set video quality
  ``ani-cli -q 360``

By default `ani-cli` would try to get the best video quality available  
You can give specific qualities like `360/480/720/..`

You can also use special names:

* `best`: Select the best quality available
* `worst`: Select the worst quality available

Multiple episodes can be viewed/downloaded by giving the episode range like so

  Choose episode [1-13]: 1 6

This would open/download episodes 1 2 3 4 5 6

## Dependencies

* grep
* curl
* sed
* mpv
* brew

## Misc

- Windows instructions can be found in this branch https://github.com/pystardust/ani-cli/tree/windows-vlc
