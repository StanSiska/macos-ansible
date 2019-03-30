#  MacOS Mojave: Ansible Playbook

The ansible playbook shall be used after clean install of MacOS to set everything up. Contains development tools installed via `Homebrew`.

## Roles/Tasks

- Installs Homebrew packages and app casks (Role `homebrew`)
- Installs App Store apps with [`mas-cli`](https://github.com/mas-cli/mas) (Role `mas`)
- Modifies MacOS settings (Role `settings`)
- Changes the user shell, if configured (Role `shell`)

## Installation

1. Install [Homebrew](https://brew.sh).
2. Install [Ansible](http://docs.ansible.com/intro_installation.html).
3. Copy `default.config.yml` to `config.yml` and edit the configuration to your likings.
   - **Don't skip this, otherwise your computer will be provisioned like mine :)**
4. Run `ansible-playbook main.yml`. Enter your account password when prompted.
   - If you have a configuration stored elsewhere (e.g. in a dotfiles folders), run `ansible-playbook main.yml --extra-vars=@/path/to/my/config.yml`

## Tools 

- aerial
- aws-sdk
- azure-cli
- calibre
- Google Chrome
- Consul
- Docker
- Firefox
- Go
- google-cloud-sdk
- itsycal Calendar
- java
- jq
- Kubernetes-cli
- Kubernetes-helm
- MacPass
- Minikube
- NodeJS
- Nomad
- Packer
- Prometheus
- Skype
- Spectacle
- Terraform
- Transmit
- Text Wrangler
- Visual Studio Code
- Unarchiver
- Unrar
- Vault
- Virtualbox
- VLC
- wget

## Acknowledgements
This playbook was created based on: [Jeff Geerling's mac-dev-playbook](https://github.com/geerlingguy/mac-dev-playbook).
Additional env commands were used from: [mathiasbynens Dotfiles](https://github.com/mathiasbynens/dotfiles/edit/master/.macos) and [olafhartong .osx](https://github.com/olafhartong/osx-defaults/blob/master/.osx)
