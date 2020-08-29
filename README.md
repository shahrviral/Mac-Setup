# Mac-Configs


## Fonts
* FiraCode: https://github.com/tonsky/FiraCode
* MesloLGS NF: https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k


## Softwares

### Utilities
* Enpass: Offline cloud agnostic password panager https://www.enpass.io/
    * Alternative: Bitwarden: Open source password manager https://bitwarden.com/
* Authy: 2FA manager https://authy.com/
* AppCleaner: App to completely uninstall other applications https://freemacsoft.net/appcleaner/
* KeyboardCleanTool: Temporarily disable keyboard to wipe clean https://folivora.ai/keyboardcleantool
* Docky: Edit dock animations https://dockey.publicspace.co/
* Encrypto: Securily encrypt files and folders with a password https://macpaw.com/encrypto
* Cryptomator: Create secure vaults https://cryptomator.org/
* Rectangle: Add support for window snapping and keyboard shortcuts for window positioning
* Amphetemine: Prevent mac from going to sleep https://apps.apple.com/us/app/amphetamine/id937984704?mt=12
* Alfred: Spotlight replacement with extra features https://www.alfredapp.com/
* Keka: Compress and Uncompress Archives https://www.keka.io/en/
    * Alternative: The Unarchiver: Compress and Uncompress Archives https://theunarchiver.com/
* IINA: Video Player https://iina.io/
* Dozer: Hide menubar icons https://github.com/Mortennn/Dozer
* Finicky: Open links in browsers based on rules https://github.com/johnste/finicky
    * Alternative: Browserosaurus: Prompt browser selection when opening links https://browserosaurus.com/
* NameChanger: Batch rename files https://mrrsoftware.com/namechanger/
* Syncthing: Encrypted host to host file synchronization https://syncthing.net/
* Transmit: Remote / Local file browser and transfer app https://panic.com/transmit/
    * Alternative: Forklift Remote / Local file browser and transfer app https://binarynights.com/
* Unclutter: Clipboard manager https://unclutterapp.com/panels/clipboard
    * Alternative: Maccy: Clipboard manager https://maccy.app/
* PopClip: Automatic tooltip on selection https://pilotmoon.com/popclip/
* FUSE for macOS: File system integration software https://osxfuse.github.io/
    
### Communication: 
* Whatsapp: https://www.whatsapp.com/download/
* Telegram: https://telegram.org/
* Discord: https://discord.com/
* Slack: https://slack.com/

### Browsers
* Brave Browser: Chromium based privacy web browser https://brave.com/
* Firefox Browser: Secure web browser https://www.mozilla.org/en-US/firefox/

### Development
* IntelliJ Idea: Java / Kotlin IDE https://www.jetbrains.com/idea/
* Webstorm: Javascript IDE https://www.jetbrains.com/webstorm/
* PyCharm: Python IDE https://www.jetbrains.com/pycharm/
* DataGrip: Database IDE https://www.jetbrains.com/datagrip/
* VS Code: Text editor https://code.visualstudio.com/
* ITerm 2: Customizable terminal emulator https://iterm2.com/
* Fork: Git repository manager https://git-fork.com/
* Postman: Rest client https://www.postman.com/
* Docker: Docker for desktop https://hub.docker.com/editions/community/docker-ce-desktop-mac/
* Kitematic: Docker container manger https://kitematic.com/
* Firefox Developer Edition: Development browser https://www.mozilla.org/en-US/firefox/developer/
* Figma: Web design tool https://www.figma.com/

## Command Line

### XCode Command Line Tools
* XCode Command Line Tools: Essential tools `xcode-select --install`

### Homebrew
* Homebrew: Command line applications manager https://brew.sh/

#### Commands
* `brew leaves` List user installed packages
* `brew leaves | xargs brew deps --installed --for-each | sed "s/^.*:/$(tput setaf 4)&$(tput sgr0)/"\`: List user installed packages and their dependencies
* `brew cask leaves | xargs brew deps --installed --for-each | sed "s/^.*:/$(tput setaf 4)&$(tput sgr0)/"\n`: List user installed cask packages and their dependencies

#### Packages
* ffmpeg: Manipulate audio and video `brew install ffmpeg`
* git: Git version control `brew install git`
* gradle: Gradle dependency management `brew install gradle`
* httpie: CLI rest client `brew install httpie`
* jenv: Manage java installations `brew install jenv`
* rename: Perl powered renamer `brew install rename`
* the_silver_searcher: Fast file search `brew install the silver searcher`
* trash: Move files to trash `brew install trash`
* tree: List directory trees `brew install tree`
* vim: Vim text editor `brew install vim`
* watch: Periodically execute command `brew install watch`
* wget: Internet file retriever `brew install wget`
* yajl: CLI json manipulation `brew install yajl`
* youtube-dl: Internet video downloader `brew install youtube-dl`
* python: Python language `brew install python@<version>`

##### Kubernetes
* yq: yaml document processor `brew install yq`
* kubernetes-cli: Manage Kubernetes clusters `brew install kubernetes-cli`
* helm: Helm deployments manager `brew install helm`

#### Taps
* AdoptOpenJDK Tap: Repository for openjdk casks `brew tap AdoptOpenJDK/openjdk`

#### Casks
* adoptopenjdk11: OpenJDK 11`brew cask install adoptopenjdk11`
* adoptopenjdk8 OpenJDK 8`brew cask install adoptopenjdk8`

### Oh My Zsh
* Oh-My-Zsh: Zsh shell customizer https://ohmyz.sh/#install
* powerlevel10k/powerlevel10k: Oh My Zsh Theme: https://github.com/romkatv/powerlevel10k#oh-my-zsh
* plugins: Add useful plugins: `plugins=(git osx web-search kubectl z zsh-autosuggestions zsh-syntax-highlighting aws jira wac)` in `~/.zshrc`

### NVM
* nvm: Node version manager https://github.com/nvm-sh/nvm#installing-and-updating

### Aliases
* Youtube Downloader
    * `alias ytdl='youtube-dl '`
* Brew Aliases
    * `alias brewup='brew update; brew upgrade; brew cleanup -s; brew doctor'`
* Python Aliases
    * `alias python='python3'`
    * `alias pip='pip3'`
    * `alias activate='source venv/bin/activate'`
    * `alias venv='python -m venv venv && source venv/bin/activate && pip install --upgrade pip'`
* Gradle Alias
    * `alias gw='./gradlew'`
* Misc Aliases
    * `alias watch='watch '`
    * `alias usage='du -h -d1'`
    * `alias runp="lsof -i "`

### Kubernetes Krew
* Krew: Kubectl Plugin manager https://krew.sigs.k8s.io/docs/user-guide/setup/install/

#### Plugins
* ns: Configure namespace for cluster `kubectl krew install ns`
* tail: Tail logs in cluster `kubectl krew install tail`


## Extensions

### Firefox
* uBlock Origin: Ad blocker https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/
* SponsorBlock: Skip Youtube sponsor segments https://addons.mozilla.org/en-US/firefox/addon/sponsorblock/
* Privacy Badger: Tracker blocker https://addons.mozilla.org/en-US/firefox/addon/privacy-badger17/
* Decentraleyes: Prevent CDN level tracking https://addons.mozilla.org/en-US/firefox/addon/decentraleyes/
* HTTPS Everywhere: Automatically update connections to HTTPS https://addons.mozilla.org/en-US/firefox/addon/https-everywhere/
* Firefox Multi-Account Containers: Isolated cookie session containers: https://addons.mozilla.org/en-US/firefox/addon/multi-account-containers/
* Facebook Container: Isolated container for Facebook https://addons.mozilla.org/en-US/firefox/addon/facebook-container/
* Temporary Containers: Create short lived containers https://addons.mozilla.org/en-US/firefox/addon/temporary-containers/
* Reddit Enhancement Suite: Reddit customizations https://addons.mozilla.org/en-US/firefox/addon/reddit-enhancement-suite/
* Tabliss: Elegant customizable new tabs https://addons.mozilla.org/en-US/firefox/addon/tabliss/
* View Image: Restore Google View Image button https://addons.mozilla.org/en-US/firefox/addon/view-image/
* Cookies.txt: Export cookies https://addons.mozilla.org/en-US/firefox/addon/cookies-txt/
* Dark Reader: Change website to dark theme https://addons.mozilla.org/en-US/firefox/addon/darkreader/

### Brave
* uBlock Origin: Ad blocker https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm
* SponsorBlock: Skip Youtube sponsor segments https://chrome.google.com/webstore/detail/sponsorblock-for-youtube/mnjggcdmjocbbbhaepdhchncahnbgone
* Privacy Badger: Tracker blocker https://chrome.google.com/webstore/detail/privacy-badger/pkehgijcmpdhfbdbbnkijodmdjhbjlgp
* View Image: Restore Google View Image button https://chrome.google.com/webstore/detail/view-image/jpcmhcelnjdmblfmjabdeclccemkghjk
* Decentraleyes: Prevent CDN level tracking https://chrome.google.com/webstore/detail/decentraleyes/ldpochfccmkkmhdbclfhpagapcfdljkj
* Reddit Enhancement Suite: Reddit customizations https://chrome.google.com/webstore/detail/reddit-enhancement-suite/kbmfpngjjgdllneeigpgjifpgocmfgmb
* Dark Reader: Change website to dark theme https://chrome.google.com/webstore/detail/dark-reader/eimadpbcbfnmbkopoojfekhnkhdbieeh



## Custom Configs

### Firefox:
* Enable Smooth Pinch Zooming: `apz.allow_zooming=true`

### Iterm2
* Use Minimal theme: Appearance > General > Theme > Minimal
* Open new tabs in current directory: Profiles > General > Working Directory > Reuse previous session's directory
* Use vertical cursor bar: Profiles > Text > Cursor > Vertical bar
* Enable blinking cursor: Profiles > Text > Cursor > Blinking cursor
* Use MesloLGS NF font: Profiles > Text > Font > MesloLGS NF
* Enable window transparency: Profiles > Window > Window Transparency > 25%
* Enable unlimited scrollback: Profiles > Terminal > Scrollback Buffer > Unlimited scrollback
* Turn off sound bell notification: Profiles > Terminal > Notifications > Silence bell
* User Natural Text Editing key bindings: Profiles > Keys > Key Mappings > Presets > Natural Text Editing



## VS Code Extensions
* Auto Close Tag by Jun Han: Automatically add html/xml closing tags
* Auto Rename Tag by Jun Han: Automatically rename paired html/xml tags
* Bracket Pair Colorizer by CoenraadS: Color code matching brackets
* indent-rainbow by oderwat: Add colors to different indentations
* Text Power Tools by Daniel Tar: Powerfull text manipulation
* Git Lens--Git supercharged by Eric Anidui: Add advanced Git capabilities
* ESLint by Dirk Baeumer: ESLint JavaScript integration
* JavaScript (ES6) code snippets by charalampos karypidis: Code snippets for JavaScript in ES6 syntax
* Live Server by Ritwick Dey: Launch local development server with live reload
* Paste JSON as Code by quicktype: Copy JSON and generate classes/types in various languages
* Prettier - Code formatter by Prettier: Code formatter
* vscode-icons by VSCode Icons Team: Icons for VS Code
* Todo+: Manage todo text based todo lists


## IntelliJ Idea Plugins
* Rainbow Brackets: Color code matching brackets https://plugins.jetbrains.com/plugin/10080-rainbow-brackets/
* Material Theme UI: Add support for Material Theme https://plugins.jetbrains.com/plugin/8006-material-theme-ui/
* Atom Material Icons: Add support for Material Icons https://plugins.jetbrains.com/plugin/10044-atom-material-icons/
* Kotlin: Kotlin language support https://plugins.jetbrains.com/plugin/6954-kotlin/


## Global Node Packages
* typescript: Add support for Typescript `npm i -g typescript`
* ts-node-dev: Add support for hot reloading typescript `npm i -g ts-node-dev`
