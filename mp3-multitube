#!/bin/bash

FILE_NAME=$1
TOTAL_MUSICS=$(wc -l < $FILE_NAME)
TOTAL_MUSICS=$((TOTAL_MUSICS+1))
DOWNLOADES_MUSICS=0

echo -e "Starting MP3 MultiTube! $TOTAL_MUSICS music(s) to download!\n"
{ cat $FILE_NAME; echo; } | while read url; do
	DOWNLOADES_MUSICS=$((DOWNLOADES_MUSICS+1))
	echo -n "Downloading ${DOWNLOADES_MUSICS}/$TOTAL_MUSICS ..."
	sudo youtube-dl --extract-audio --audio-format mp3 --audio-quality 0 $url >> /tmp/log.youtube-dl
	echo  " done!"
done
echo -e "\nFinish! You have $DOWNLOADES_MUSICS new music(s)!"