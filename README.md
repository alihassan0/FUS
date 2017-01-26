
## Snippets

### ffmpeg
| property         | Value           |
| ------------- |:-------------:| 
| purpose      | convert images to videos |
| source      | https://trac.ffmpeg.org/wiki/Slideshow |
| snippets | `ffmpeg -framerate 8 -i %04d.jpg output.mp4` |
| Notes | images must be sequntionally in order  |

### nginx
| property         | Value           |
| ------------- |:-------------:| 
| purpose      | edit configuration file |
| snippets | `sudo nano /etc/nginx/sites-available/default` |
| Notes | must restart for changes to take effect  |

| property         | Value           |
| ------------- |:-------------:| 
| purpose      | restart nginx to update config  |
| snippets | `sudo service nginx restart` |

## scritps

### renameImages
`renames images to sequential order`

```bash
a=1
for i in *.jpg; do
  new=$(printf "%04d.jpg" "$a") #04 pad to length of 4
  mv -- "$i" "$new"
  let a=a+1
done
```


