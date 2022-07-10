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

## 3. When configuring Mysql Server, meet "ERROR 1698 (28000): Access denied for user 'root'@'localhost'"
[Solution](https://stackoverflow.com/questions/39281594/error-1698-28000-access-denied-for-user-rootlocalhost)
> There are two ways to solve this:
>
> 1. You can set the root user to use the mysql_native_password plugin
> 2. You can create a new db_user with you system_user (recommended)

## 3.5 When finished the User and Password problem, meet "Can't connect to local MySQL server through socket '/var/lib/mysql/mysql.sock' (2)"
[Solution](https://stackoverflow.com/questions/4448467/cant-connect-to-local-mysql-server-through-socket-var-lib-mysql-mysql-sock)
> Ensure that your mysql service is running
>
>> service mysqld start