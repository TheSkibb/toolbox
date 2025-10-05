# Windows caps lock to ctrl

~~~powershell
$hexified = "00,00,00,00,00,00,00,00,02,00,00,00,1d,00,3a,00,00,00,00,00".Split(',') | % { "0x$_"};

$kbLayout = 'HKLM:\System\CurrentControlSet\Control\Keyboard Layout';

New-ItemProperty -Path $kbLayout -Name "Scancode Map" -PropertyType Binary -Value ([byte[]]$hexified);
~~~

([from](https://gist.github.com/joshschmelzle/5e88dabc71014d7427ff01bca3fed33d))
