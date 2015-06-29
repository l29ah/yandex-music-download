Yandex Music Downloader
=====================

This is a simple command line Perl script for downloading music from Yandex Music (http://music.yandex.ru).
Origin of the script is the following article: http://kaimi.ru/2013/11/yandex-music-downloader/

# Usage

```bat
ya.pl [-adkpt] [long options...]
	-p --playlist     playlist id to download
	-k --kind         playlist kind (eg. ya-playlist, music-blog,
	                  music-partners, etc.)
	-a --album        album to download
	-t --track        track to download (album id must be specified)
	-d --dir          download path (current direcotry will be used by
	                  default)
	--proxy           HTTP-proxy (format: 1.2.3.4:8888)
	--exclude         skip tracks specified in file
	--include         download only tracks specified in file

	--debug           print debug info during work
	--help            print usage

	--include and --exclude options use weak match i.e. ~/$term/

	Example:        
		ya.pl -p 123 -k ya-playlist
		ya.pl -a 123   
		ya.pl -a 123 -t 321

```

For further assistance don't hesitate to ask for help in GitHub issues or on the blog: http://kaimi.ru