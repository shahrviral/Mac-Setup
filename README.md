# Mac-Configs


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
    * Alternative: Remote / Local file browser and transfer app https://binarynights.com/
* Unclutter: Clipboard manager https://unclutterapp.com/panels/clipboard
    * Alternative: Maccy: Clipboard manager https://maccy.app/
* PopClip: Automatic tooltip on selection https://pilotmoon.com/popclip/
    
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
* helm: Helm deployments manager `brew install helm`
* httpie: CLI rest client `brew install httpie`
* jenv: Manage java installations `brew install jenv`
* kubernetes-cli: Manage Kubernetes clusters `brew install kubernetes-cli`
* rename: Perl powered renamer `brew install rename`
* the_silver_searcher: Fast file search `brew install the silver searcher`
* trash: Move files to trash `brew install trash`
* tree: List directory trees `brew install tree`
* vim: Vim text editor `brew install vim`
* watch: Periodically execute command `brew install watch`
* wget: Internet file retriever `brew install wget`
* yajl: CLI json manipulation `brew install yajl`
* youtube-dl: Internet video downloader `brew install youtube-dl`
* yq: yaml document processor `brew install yq`

#### Taps
* AdoptOpenJDK Tap: Repository for openjdk casks `brew tap AdoptOpenJDK/openjdk`

#### Casks
* adoptopenjdk11: OpenJDK 11`brew cask install adoptopenjdk11`
* adoptopenjdk8 OpenJDK 8`brew cask install adoptopenjdk8`

### Oh My Zsh
* Oh-My-Zsh: Zsh shell customizer https://ohmyz.sh/#install
* powerlevel10k/powerlevel10k: Oh My Zsh Theme: https://github.com/romkatv/powerlevel10k#oh-my-zsh
* plugins: Add useful plugins: `plugins=(git osx web-search kubectl z zsh-autosuggestions zsh-syntax-highlighting aws jira wac)` in `~/.zshrc`

### Krew
* Krew: Kubectl Plugin manager https://krew.sigs.k8s.io/docs/user-guide/setup/install/

#### Plugins
* ns: Configure namespace for cluster `kubectl krew install ns`
* tail: Tail logs in cluster `kubectl krew install tail`

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
