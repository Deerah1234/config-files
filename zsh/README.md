# My Zsh Cofiguration

This repository contains my personal configuration file for Zsh. It includes various settings, aliases, and plugins that I find useful.

## Getting Started

To use my Zsh configuration, follow these steps:

1. Clone this repository:
	```bash
	git clone https://github.com/[username]/zsh-config.git ~/.zsh-config
	```
2. Install Oh My Zsh:
	```bash
	sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
	```
3. Create a symbolic link to the .zshrc file in this repository:
	```bash
	ln -s ~/.zsh-config/.zshrc ~/.zshrc
	```
4. Install the required plugins:
	- zsh-autosuggestions: Install it by running
		```bash
		git clone https://github.com/zsh-users/zsh-autosuggestions ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions
		```
	- zsh-syntax-highlighting: Install it by running
		```bash
		git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ~/.oh-my-zsh/custom/plugins/zsh-syntax-highlighting
		```
	- logo-ls: Install it by running
		```bash
		npm install --global logo-ls
		```

Once installed, add the plugin names to the plugins array in your ~/.zshrc file:
```bash
plugins=(
  git
  zsh-autosuggestions
  zsh-syntax-highlighting
)
```

5. Install the required font:

	- **MesloLGS NF Regular**: Download and install the font from [here](https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k).

6. Install Powerlevel10k:
	```bash
	git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/.oh-my-zsh/custom/themes/powerlevel10k
	```
	Then set the ZSH_THEME variable in your ~/.zshrc file to powerlevel10k/powerlevel10k:
	```bash
	ZSH_THEME="powerlevel10k/powerlevel10k"
	```
7. Finally, run the following command to refresh your Zsh configuration:
	```bash
	source ~/.zshrc
	```

## Customization
To customize Powerlevel10k prompt, run 
```bash
p10k configure.
```
To customize aliases, open the **~/.zshrc** file and add or modify aliases as needed. My aliases can be found towards the bottom of the file.
To customize the **logo-ls** colors, run 
```bash
logo-ls --config
```
and modify the JSON file that is generated.

## Feedback

Feel free to open an issue if you have any questions or suggestions.
