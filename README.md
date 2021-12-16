# Terminal-Setup-Guide-with-Zsh-Awesomeness-on-UBUNTU
how I setup my Linux terminal and the tools that I use.

# At first we need to run this command
~~~
sudo apt-get update && sudo apt-get upgrade
~~~

# First thing first need to install ZSH Shell
~~~
sudo apt install zsh
~~~

# After that close the terminal & re-opened the terminal. So when you install the zsh and start your shell for the first time it finds that you don't have a valid cshrc file and then it will show you this configuration wizard so either you can go through this you can press 0. Next thing you usually do is install OH MY ZSH. But before this we need to install git.
~~~
sudo apt install -y git
~~~

# After that run this command
~~~
sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
~~~

# Install Zsh autosuggestions
~~~
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
~~~

# Open the .zsh file and replace plugins
~~~
plugins=(git zsh-autosuggestions)
~~~

# Install Zsh syntax highlighting
~~~
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
~~~

# Again open the .zsh file and replace plugins
~~~
plugins=(git zsh-autosuggestions zsh-syntax-highlighting)
~~~

## After that close the terminal & reopened the terminal

# Install font awesome package
~~~
sudo apt install -y fonts-font-awesome
~~~

# Install powerlevel-10k
~~~
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
~~~

# Open .zsh file & replace the line with
~~~
ZSH_THEME="powerlevel10k/powerlevel10k"
~~~

## After that close the terminal & reopened it & you can see the configuration wizard. Answer the few questions & customize the terminal as you want.