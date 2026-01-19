# `video`  and `audio`
* src= describes the source / path , need not to be on the local machine
* **loop, autoplay, muted**
* controls gives options to download , play etc
* poster is like a thumbnail
* `preload` to control whether to download info or not

## preload Attribute

Tells browser how much media to load before play
Used with <audio> and <video>

### Values:

* none → load nothing
* metadata → load info only (best choice)
* auto → load full media

# SVG (Scalable Vector Graphics)

Vector-based (does not lose quality)
Best for icons, logos

## SVG using <img>

Alternate way to use SVG
xmlns not required
```html
<img src="icon.svg" alt="icon">
```

# <iframe>

* Used to embed external content
* Commonly used for YouTube videos