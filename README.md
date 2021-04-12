# Portfolio
Portfolio of a few of my side projects and my professional work

![Screenshot](https://raw.githubusercontent.com/NathanielWroblewski/portfolio/master/screenshot1.png)
---
![Screenshot](https://raw.githubusercontent.com/NathanielWroblewski/portfolio/master/screenshot2.png)

Assets
===

Images are hosted on S3 via a CDN.  Currently, I resize each image for better
site load speeds and for better quality depending on the device resolution.

I snap a screenshot around 1440 × 898 and then I resize with ffmpeg for different scenarios.

For mobile:
```
ffmpeg -i ./lavabits.png -vf scale=620:387 ./mobile/lavabits.png
```

For retina mobile:
```
ffmpeg -i ./lavabits.png -vf scale=720:449 ./retina_mobile/lavabits.png
```

For thumbnails:
```
ffmpeg -i ./lavabits.png -vf scale=310:184 ./resized/lavabits.png
```

For retina thumbnails:
```
ffmpeg -i ./lavabits.png -vf scale=620:387 ./retina_thumbnails/lavabits.png
```
