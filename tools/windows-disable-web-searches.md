# windows disable web searches

[source](https://www.tomshardware.com/how-to/disable-windows-web-search)

create new registry key in `HKEY_CURRENT_USER\Software\Policies\Microsoft\Windows` called Explorer

in the key create a DWORD called `DisableSearchBoxSuggestions` and give it the value 1



