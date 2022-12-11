# mp32mp4-lq

This dirty script is to convert my mp3 collection to aac with the lowest possible bitrare while keeping some decent quality,
useful if you want to stream your collection from airsonic to your car through your mobile data connection.

It uses the NeroAacEnc and NeroAacTag programs freely released by Nero for the Linux platform. Reason being at the time of
creating this script NeroAacEnc was the best by far encoder for aac music files.
This script also depends on lame to decode mp3 files, and on ffprobe, part of ffmpeg, to extract metadata from mp3 files.

You can download NeroAAC free utilities from https://web.archive.org/web/20160923100008/http://ftp6.nero.com/tools/NeroAACCodec-1.5.1.zip
 
I use Guayadeque, https://guayadeque.org , to keep my music collection organized. My collection is structured as
Album Artist/Album Name/CD#(if exists)/Song#-Title.mp3
Guayadeque will also save the album cover as cover.jpg and place it along with the song files.

This script will convert all music to aac files, and embed as much data as possible in those files.

This script is to be run with an only argument: the music directory in which all your mp3 files are located. It can
be run again and will only update new mp3 files keeping the previously converted to aac 

This script could be greatly improved with things like error detection and better file name handling.
