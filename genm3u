#!/bin/bash
# Made with <3 by @maakhai
# Version: 0.2

arquivo="$2.m3u"
extensoes_audio="mp3 flac aac ogg"
extensoes_video="mp4 mkv avi"
mensagem_de_uso="usage: $0 <command> <playlist_name>
\n\n
-a | --audio\n
-v | --video   
"

if [ -z "$2" ]; then
  	arquivo="playlist.m3u"
fi

cria_playlist(){
  for ext in $1; do
    ls -1v *.$ext 2> /dev/null >> $arquivo
  done
}

case $1 in 
  -a | --audio) 
    cria_playlist "$extensoes_audio"
    ;;
  -v | --video)
    cria_playlist "$extensoes_video"
    ;;
  *)
    echo -e $mensagem_de_uso
    exit
    ;;
esac

if [ -f "$arquivo" ]; then
  echo "completed ✨ 🌟 ✨"
else
  echo "the operation failed."
fi
