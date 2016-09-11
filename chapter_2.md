### Eloquent JavaScript, Chapter 3: Functions
#### Exercise 1: Minimum

<iframe src="https://www.livecoding.tv/mikeumus/videos/5v0ne/embed" width="560" height="315" frameborder="0" allowfullscreen="true" scrolling="no"></iframe>

The previous chapter introduced the standard function Math.min that returns its smallest argument. 
We can do that ourselves now. Write a function min that takes two arguments and returns their minimum.

```
console.log(min(0, 10));
// → 0
console.log(min(0, -10));
// → -10
```

#### Exercise Code:
{%ace edit=true, lang='javascript'%}
(function(){ // This is our self invoking closure. We do this to keep the global environment pure. 
	
	// Long obvious answer: 
	function min(arg1, arg2){
		if(arg1 < arg2){
			return arg1;
		} else{
			return arg2;
		}
	}	
	console.log(min(0, 10));
	console.log(min(0, -10));

})();
{%endace%}
