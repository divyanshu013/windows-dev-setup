<header align="center">
    <div align="center">
        <img src="icon.png" alt="Logo" width="250" />
    </div>
    <h1 align="center">Windows Dev Setup</h1>
    <p align="center">A developer guide for people coming from macOS and Linux</p>
</header>



## Coding related

- [VS Code](https://code.visualstudio.com/Download) - code editor

- [Cascadia Code](https://github.com/microsoft/cascadia-code) - font

- Terminal
  - [Microsoft Terminal](https://www.microsoft.com/en-us/p/windows-terminal/9n0dx20hk701?activetab=pivot:overviewtab) - not as customizable yet but leaner on memory
  - [Fluent Terminal](https://www.microsoft.com/en-us/p/fluent-terminal/9p2krlmfxf9t?cid=storebadge&ocid=badge&rtc=1&activetab=pivot:overviewtab) - better in features than Microsoft's currently but consumes slightly more memory (using this for now)

- [Setup WSL](https://github.com/michaeltreat/Windows-Subsystem-For-Linux-Setup-Guide) and [update to WSL2](https://docs.microsoft.com/en-us/windows/wsl/install-win10#update-to-wsl-2) - Windows Subsystem for Linux is not a VM or dual boot, it's a native POSIX (Portable Operating System Interface Interface) that mounts directly to Windows' file system.

  - VSCode once opened (from GUI or via `code` command) will prompt to install the [WSL extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl)

  - **Note**: keep your code in native linux filesystem (i.e. inside `/home/<user>` directory) because WSL2 has [some](https://docs.microsoft.com/en-us/windows/wsl/compare-versions) [known issues](https://github.com/microsoft/WSL/issues/4197) with [cross OS filesystem performance](https://vxlabs.com/2019/12/06/wsl2-io-measurements/)

  - **Troubleshooting**: quite rarely connection to `WSL: Ubuntu` drops from VSCode, the solution is to restart WSL. From powershell run `wsl --shutdown` and restart VSCode

- Setup `git`

  ```sh
  git config --global user.name "First Last"
  git config --global user.email email@email.com
  ```

- Add [GPG](https://help.github.com/en/articles/managing-commit-signature-verification) and [SSH](https://help.github.com/en/articles/connecting-to-github-with-ssh) keys (still exploring how to integrate the passphrases with keychain so you don't have to type them on each login)

- Install `build-essential`



## CLI

- Install Zsh
- Install [Oh my ZSH](https://github.com/robbyrussell/oh-my-zsh)
- Install [GitHub CLI tool](https://github.com/cli/cli)



### CLI plugins

- [ZSH autosuggestions](https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md)
- [bgnotify](https://github.com/robbyrussell/oh-my-zsh/tree/master/plugins/bgnotify)
- [ZSH syntax highlighting](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md)
- [z](https://github.com/robbyrussell/oh-my-zsh/tree/master/plugins/z)
- [fzf](https://github.com/junegunn/fzf)
- [fkill-cli](https://github.com/sindresorhus/fkill-cli)
- [fx](https://github.com/antonmedv/fx)
- [bat](https://github.com/sharkdp/bat#on-ubuntu-using-apt)
- [diff-so-fancy](https://github.com/so-fancy/diff-so-fancy)
- [ag](https://github.com/ggreer/the_silver_searcher)
- [sudo](https://github.com/robbyrussell/oh-my-zsh/tree/master/plugins/sudo)
- [yt-dlp](https://github.com/yt-dlp/yt-dlp) - `youtube-dl` improved



## Tools

- [Quick Look](https://github.com/QL-Win/QuickLook) - quick look for windows, just press <kbd>Space</kbd>, has [some plugins](https://github.com/QL-Win/QuickLook/wiki/Available-Plugins)
- [Ditto](https://www.microsoft.com/en-us/p/ditto-clipboard/9nblggh3zbjq?activetab=pivot:overviewtab#) - clipboard manager
- [Twinkle Tray](https://twinkletray.com/) - brightness control for external monitors
- [Power Toys](https://github.com/microsoft/PowerToys) - utilities such as color picker, window management, image resizer, preview pane, run (Alfred / Albert alternative)
- [Iriun](https://iriun.com/) - use your phone as camera
- [WOMic](https://wolicheng.com/womic/) - use your phone as microphone
- [DroidCam](http://www.dev47apps.com/) - features both camera and microphone functionality
- [Croc](https://github.com/schollz/croc) - CLI file transfer
- [Unison](https://apps.microsoft.com/store/detail/intel%C2%AE-unison%E2%84%A2/9PP9GZM2GN26) - easily transfer media to / from iPhone



## Tips

- **Emoji picker**: use <kbd>Super</kbd> + <kbd>.</kbd>
- **App switcher**: use <kbd>Super</kbd> + <kbd>Number key</kbd>
- It's possible to copy some output into Windows' clipboard by piping output to `clip.exe` for example `echo 'GG' | clip.exe`, not sure if there's a way to paste yet



## Apps

- [Typora](https://typora.io/) - markdown editor
- [MarkText](https://github.com/marktext/marktext) - open source markdown editor
- [Notion](https://notion.so) - notes and wiki + [addon](https://github.com/dragonwocky/notion-enhancer)
- [Firefox](https://www.mozilla.org/en-US/firefox/new/) - web browser
- [Brave](https://brave.com/download/) - alt web browser
- [Steam](https://store.steampowered.com/) - games
- [Discord](https://discord.com/new) - chats
- [Telegram](https://telegram.org/) - chats
- [Spotify](https://www.spotify.com/in/download/windows/) - music
- [Studio One](https://www.presonus.com/products/Studio-One) - DAW
- [Davinci Resolve](https://www.blackmagicdesign.com/products/davinciresolve/) - video editing
- [Insomnia](https://insomnia.rest/download/#windows) - REST client
- [Beekeeper Studio](https://github.com/beekeeper-studio/beekeeper-studio) - DB GUI
- [RunJS](https://runjs.dev/) - JS run environment
- [MusicXMatch](https://www.microsoft.com/en-us/p/musixmatch-lyrics-sing-along-spotify-itunes-windows-media-player/9wzdncrfj235?activetab=pivot:overviewtab) - lyrics
- [Figma](https://www.figma.com/downloads/) - design
- [Boss Tone Studio](https://www.boss.info/global/products/gt-1/downloads/) - guitar processor software
- [Tunnel Bear](https://www.tunnelbear.com/apps/windows) - VPN
- [Remembear](https://www.remembear.com/download) - password manager
- [Zoom](https://zoom.us/download#client_4meeting) - video meetings
- [VLC](https://www.microsoft.com/en-us/p/vlc/9nblggh4vvnh?activetab=pivot:overviewtab) - media player
- [Pym](https://www.microsoft.com/en-us/p/pym/9pmtmrnbxmpb?activetab=pivot:overviewtab) - image compression
- [Authy](https://www.microsoft.com/en-us/p/pym/9pmtmrnbxmpb?activetab=pivot:overviewtab) - 2FA client
- [Flip clock](https://fliqlo.com/#/screensaver) - screensaver
- [Lively](https://github.com/rocksdanister/lively) - use anything as wallpaper
- [Files](https://github.com/files-community/Files) - better file explorer



## Related

- [Linux dev setup](https://github.com/divyanshu013/linux-dev-setup)
- [Mac dev setup](https://github.com/divyanshu013/mac-dev-setup)
- [Dotfiles](https://github.com/divyanshu013/dotfiles)

Icon from [icons8](https://icons8.com)
