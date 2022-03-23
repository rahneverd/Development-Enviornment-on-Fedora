# Development-Enviornment-on-Fedora
Guide to setting up development enviornment on Fedora

01) Updating OS
  sudo dnf update
  sudo dnf upgrade
  
02) Theme and Icons Theme
  Arc-Fatabulous
    sudo dnf install autoconf
    sudo dnf install automake
    sudo dnf install sassc
    sudo dnf install pkgconf-pkg-config
    sudo dnf install git
    sudo dnf install optipng.x86_64
    sudo dnf install inkscape
    sudo dnf install gtk3
    sudo dnf install gtk3-devel
    sudo dnf install gnome-themes-extra
    sudo dnf install gtk-murrine-engine
    sudo dnf install gettext-devel
    sudo dnf install libtool
    mkdir Themes
    cd Themes
    git clone https://github.com/andreisergiu98/arc-flatabulous-theme --depth 1 && cd arc-flatabulous-theme
    ./autogen.sh --prefix=/usr
    sudo make install
    
    Alternatively arc theme can also be used from OpenSuse
    sudo dnf config-manager --add-repo https://download.opensuse.org/repositories/home:Horst3180/Fedora_25/home:Horst3180.repo
    sudo dnf install arc-theme
  Paper
    sudo dnf config-manager --add-repo https://download.opensuse.org/repositories/home:snwh:paper/Fedora_25/home:snwh:paper.repo
    sudo dnf install paper-icon-theme
    
03) GNOME Plugins
    Dash to Dock
    Always Zoom Workspaces
    Auto Move Windows
    Native Window Placement
    Launch new instance
    Steal My Focus
    AlternateTab
    Window List
    Applications Menu
    Caffeine
    Clipboard Indicator
    Gistnotes
    OpenWeather
    Places Status Indicator
    System-monitor
    Todo.txt
    TopIcons Plus
    User Themes

04) Install VS Code
  sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
  cat <<EOF | sudo tee /etc/yum.repos.d/vscode.repo
  [code]
  name=Visual Studio Code
  baseurl=https://packages.microsoft.com/yumrepos/vscode
  enabled=1
  gpgcheck=1
  gpgkey=https://packages.microsoft.com/keys/microsoft.asc
  EOF
  dnf check-update
  sudo dnf install code
  
05) Installing nodejs
  sudo dnf install nodejs
  
06) Installing expo (for react native)
  npm install --global expo-cli
  
8) Installing wine and setting up office
  
  
  
