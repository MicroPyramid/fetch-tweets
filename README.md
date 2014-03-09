fetch-tweets
============

Fetch tweets using javascript

This is very straight plugin to fetch tweets using javascript.

Fetching tweets with javascrpt is not allowed by default, so i found the other way by using widget as medium.

1. Go to www.twitter.com and sign in then go to your settings page.
2. Go to "Widgets" on the left hand side.
3. Create a new widget as you like.
4. Check "exclude replies" if you dont want replies in results.
5. Now go back to settings -> widgets page, you will see the widget you just created. Click edit.
6. Now look at the URL in your web browser, you will see a long number like this: 441110970094473216.
7. Use this as your ID below!


```javascript
function tweets(tws){
		$.each(tws, function(i,o){
			// You can do as you wish with the values in 'o' objects.
			console.log(o);
		});	
	}
// this will fetch tweets of the given widget id and pass the tweets to tweets function
tw.fetch('352009122125856768', 20, tweets); 

```

I made is as simple as i can so, you can extend it as you wish. Let me know if you need any additions. 
