returns only the local ip address
~~~
ifconfig | grep -Eo 'inet (addr:)?([0-9]*\.){3}[0-9]*' | grep -Eo '([0-9]*\.){3}[0-9]*' | grep -v '127.0.0.1'
~~~

look for "inet" on wlp3s0
~~~
ifconfig
~~~
