# Import the Enabler Library

```
<script src="https://s0.2mdn.net/ads/studio/Enabler.js"></script>
```

# Wait for Enabler to be initialized
### This can be put in an "onload" function or at the bottom of the page in a script tag.

```javascript
if(Enabler.isInitialized()){
	initAd();
}
else{
	Enabler.addEventListener(studio.events.StudioEvent.INIT, initAd);
}
```

# Setup Clicktag

```javascript
Enabler.exit("clickTag", "http://www.google.com");
```

# Setup a tracked link that isn't the Click Tag

```javascript
Enabler.exit("legalLink", "http://www.weather.com.com");
```