# mp3_multitube
Multidownload MP3 musics from youtube-dl library!

### Download youtube-dl library

```bash
sudo wget http://youtube-dl.org/downloads/2013.05.01/youtube-dl -O /usr/bin/youtube-dl
sudo chmod a+x /usr/bin/youtube-dl
sudo youtube-dl -U
```
### Download to_mp3 library
```bash
sudo apt-get install libavcodec-extra-53  
```

### Extract and use

Put in your .bashrc:
```bash
export PATH=/mp3_multitube:$PATH
```

Execute:
```bash
mp3-multitube your/path/file/urls.here
```

Have fun! :)
