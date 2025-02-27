## Windows installation of git

Go to [git-scm.org](https://git-scm.com/download/win), download **Git Standalone Installer** and install it.
When installing, go through the wizard and select these options:

* Run Git from the Windows Command Prompt
* Checkout Windows-style, commit Unix-style line endings

Do not change any other options, they can be left as default.
Please ensure that **Git Credential Manager Core** option is ["checked"](https://github.com/git-ecosystem/git-credential-manager/blob/release/docs/install.md#git-for-windows-star), to install the extra tool by default with Git installation.

{{ figure( img=static('windows-git-cred-manager.png'), alt='Git installation credential manager allow', ) }}


Then set your Git editor.
If you have a terminal window open, close it, and open a new one.
(The installation changes system settings which have to be loaded again.)

In the new command line, enter:

```console
> git config --global core.editor notepad
> git config --global format.commitMessageColumns 80
> git config --global gui.encoding utf-8
```

Now continue with the rest of setup at [General Settings in Git install]({{ lesson_url('git-en/install') }}).
