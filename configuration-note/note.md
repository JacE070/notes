## 1. Cannot execute command which was installed by pip3
[Solution](https://stackoverflow.com/questions/35898734/pip-installs-packages-successfully-but-executables-not-found-from-command-line/59436732#59436732)

> The problem on Linux is that pip install ... drops scripts into ~/.local/bin and this is not on the default Debian/Ubuntu $PATH.
>
> Here's a GitHub issue going into more detail: https://github.com/pypa/pip/issues/3813
> 
> To fix, just add ~/.local/bin to your $PATH, for example by adding the following line to your .bashrc file:
>
>> export PATH="$HOME/.local/bin:$PATH"
