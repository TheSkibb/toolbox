processors: updateRecord

for ISO 8601:
~~~
${field.value:toDate("yyyy-MM-dd'T'HH:mm:ss.SSSSSS'Z'", "UTC"):toNumber()}
~~~
make sure the string with the date z


for dates on format:

2023-10-16T00:00:00+00:00

~~~
${field.value:toDate("yyyy-MM-dd'T'HH:mm:ss.SSSSSS'Z'", "UTC"):toNumber()}
~~~
