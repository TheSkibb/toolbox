# iso 8601 date in nifi expression language

~~~
${now():format("yyyy-MM-dd'T'HH:mm:ss'Z'", "GMT")}
~~~

[docs](https://nifi.apache.org/docs/nifi-docs/html/expression-language-guide.html#format)
