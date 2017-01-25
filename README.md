## FFMPEG

| property         | Value           |
| ------------- |:-------------:| 
| purpose      | convert images to vedeos |
| source      | http://ludumdare.com/compo/2013/05/01/higher-quality-video-workaround-for-chronolapse/ |
| snippets | `ffmpeg -r 20 -i “img (%d).png” -q:v 1 -b:v 1500k timelapse.mp4` |
