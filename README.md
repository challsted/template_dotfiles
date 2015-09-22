#Template Dotfiles

These dotfiles are to be very close in compairson to my main dotfiles.  
These are to be used as a "template" for others to build there own,  
and so that I can customize my own dotfiles with out fear of breaking others (as badly).  

If you use my main repo "hackinginfo/dotfiles" then your asking to use what i have :P  
Look here for the templates. 

Happy Hacking!!

## Installation

You will need git installed, and if you want to use these you will also need `vim`, `zsh`, `curl`(and/or `wget`)  
So, if your on ubuntu, you could copy this  
* `sudo apt-get install git vim zsh tmux curl wget`

Now you will need to clone my repository, I suggest that you put it inside of a folder under your home directory, i personally use a folder called "git" but this is up to you, and optional.
If you want to make a folder first you can do this:
* `mkdir -p ~/git && cd ~/git`

If you created the folder make sure you cd into it, then run the next command
* `git clone https://github.com/hackinginformation/template_dotfiles.git`

**ZSH**
* If you plan to use `zsh`, you will also need [Oh-My-Zsh][zsh]. You will need to run this to use my config:
  * `ln -sf ~/git/template_dotfiles/zsh/zshrc.symlink ~/.zshrc`
* If You plan to use the "prompt" that I created, you can copy paste this
  * `ln -sf ~/git/template_dotfiles/zsh/custom_prompt.zsh-theme ~/.oh-my-zsh/custom/prompt.zsh-theme`
* If you didnt use the ~/git folder, or you used a different one then you need to update this line, you will also need to open the ~/.zshrc and edit line number 32 to your correct path.
Once that is complete, you will need to run:
* `source ~/.zshrc` and your complete! Your zsh will change and you'll notice a few new features.

**VIM**
* If you plan to use `vim` you will need to run this to use my config:
* `ln -sf ~/git/template_dotfiles/vim/vimrc.symlink ~/.vimrc`
* If you didnt use the ~/git folder, or you used a different one then you need to update this line
Once that is complete open your vimrc in vim:

**TMUX**
* If you plan to use `tmux`, then you will need to copy my tmux.conf.
* `ln -sf ~/git/template_dotfiles/tmux/tmux.config ~/.tmux.conf`
* Open a new tmux session for validation (if you dont already have one open)
  * (for example) `tmux new -s random`

## Contact the author

Professional  Twitter [@hackinginfo][tweet]

My Blog    [masammich's][blog]


[zsh]:          https://github.com/robbyrussell/oh-my-zsh
[tweet]:        https://twitter.com/MaSammchs
[blog]:         http://masammich.technoanomaly.com/
