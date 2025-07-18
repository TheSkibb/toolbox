# Extract multiple attributes from a json flow file using jsonPath 
(this can for example be useful for evaluateJsonPath processors)

for example with this structure:
~~~json
{a: {
    aa: 1,
    ab: 2,
    ac: 3
    }
}
~~~

and you only want the aa and ac attributes from the json object you can do:

~~~
$.a['aa', 'ac']
~~~
