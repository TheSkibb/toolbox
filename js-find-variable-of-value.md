# Find a varible of a certain value

~~~js
for (let key in window) {
  if (typeof window[key] === 'string' && window[key].includes('your-token-here')) {
    console.log(key, window[key]);
  }
}
~~~
