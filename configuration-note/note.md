## 1. Cannot execute command which was installed by pip3
[Solution](https://stackoverflow.com/questions/35898734/pip-installs-packages-successfully-but-executables-not-found-from-command-line/59436732#59436732)

> The problem on Linux is that pip install ... drops scripts into ~/.local/bin and this is not on the default Debian/Ubuntu $PATH.
>
> Here's a GitHub issue going into more detail: https://github.com/pypa/pip/issues/3813
> 
> To fix, just add ~/.local/bin to your $PATH, for example by adding the following line to your .bashrc file:
>
>> export PATH="$HOME/.local/bin:$PATH"

## 2. When trying to configure Gnome Extensions, meet "Although GNOME Shell integration extension is running, native host connector is not detected. Refer documentation for instructions about installing connector."
[Solution](https://stackoverflow.com/questions/61516422/gnome-shell-integration-extension-is-running-native-host-connector-is-not-detec)

> FYI: starting from Ubuntu 21.10 Firefox comes as a default browser and as a snap, as well as Chromium.
Just use another browser.
