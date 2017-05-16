# Atom Web/Apps IDE
Include Majors dependencies, configurations, linters, languages, autocompletes, etc

### Requirements
- php
- git
- composer
- sass
- sass
If you need to install some of this dependencies hust execute the following command:
- [x] ``` wget -qO- https://raw.githubusercontent.com/7rin0/config-atom/master/bin/dependencies.sh | bash ```

### Screenshot
![Atom IDE](https://raw.githubusercontent.com/7rin0/config-atom/master/media/screenshot.png)

### Install Atom from CLI
#### Execute on Centos
- [x] ``` wget -qO- https://raw.githubusercontent.com/7rin0/config-atom/master/bin/distros/centos/atom_centos_install.sh | bash ```

#### Execute on Fedora
- [x] ``` wget -qO- https://raw.githubusercontent.com/7rin0/config-atom/master/bin/distros/fedora/atom_fedora_install.sh | bash ```

#### Execute on Ubuntu/Debian
- [x] ``` wget -qO- https://raw.githubusercontent.com/7rin0/config-atom/master/bin/distros/ubuntu-debian/atom_ubuntu-debian_install.sh | bash ```

### APM: Operations/Actions
#### Import Atom's dependencies from file
- [x] ``` apm install --packages-file packages.list ```

#### Export Atom's dependencies to file
- [x] ``` apm list --installed --bare > packages.list ```

#### Remove ALL packages
- [x] ``` apm remove $(apm list --installed --bare | cut -d'@' -f1) ```

#### Update Atom dependencies
- [x] ``` apm upgrade ```
