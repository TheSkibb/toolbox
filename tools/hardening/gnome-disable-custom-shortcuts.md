# disable user from being able to set shortcuts

add a lock file to dconf
~~~
/bin/sudo rm /etc/dconf/db/local.d/locks/00_shortcuts
~~~

[more about lockfiles](https://help.gnome.org/admin/system-admin-guide/stable/dconf-lockdown.html.en)

add a line to the file

~~~
/org/gnome/settings-daemon/plugins/media-keys/custom-keybindings
~~~

reload dconf

~~~bash
/bin/sudo dconf update
~~~
