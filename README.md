# sublimetext
Sublime Text Stable Installer for Debian

How to install :

  Open the terminal and clone the bash file
  
  sudo bash ./sublime.sh
  
- **?** If you are receiving an error saying "gpg not found" when running the code provided,it means that the gpg package is not installed on your system.
#Use ** ``` sudo apt-get install gnupg ``` ** to install gpg package.

- **?** Error called, "W: GPG error: https://packages.microsoft.com/repos/vscode stable InRelease: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY EB3E94ADBE1229CF
E: The repository 'https://packages.microsoft.com/repos/vscode stable InRelease' is not signed.
N: Updating from such a repository can't be done securely, and is therefore disabled by default.
N: See apt-secure(8) manpage for repository creation and user configuration details."
Use this comand - ``` sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys EB3E94ADBE1229CF ```

# Here are the instructions for setup terminus
- install package manager(ctrl+shift+p) and install terminus
### copy and paste these keymaps to the exact dirs
- go to Preference>Package Settings>Terminus>KeyBindings
-- [
   {
       "keys": ["ctrl+shift+t"],
       "command": "terminus_open",
       "args" : {
           "cmd": "bash",
           "cwd": "${file_path:${folder}}",
           "panel_name": "Terminus"
       }
   }
]
- go to Preference>Package Settings>Terminus>Command Palette
-- [{
    "caption": "Terminal (panel)",
    "command": "terminus_open",
    "args": {
        "cmd": "bash",
        "cwd": "${file_path:${folder}}",
        "title": "Terminal",
        "panel_name": "Terminus"
    }
}]
