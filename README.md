# SpotMyBackup
Backup and Restore your Spotify Playlists and "My Music".

This javascript based app allows you to backup all your playlists and import them in any other Spotify Account. It uses the OAuth-Functionality of Spotify to be able to handle your personal playlists. 

In consequence, no credentials or data is stored or processed on the Webserver itself.

You can use it at www.spotmybackup.com or on your own webserver (see Q&A).

## Documentation
* [Spotify Web API](https://developer.spotify.com/web-api/endpoint-reference/)

## Setup
* create new app https://developer.spotify.com/my-applications
* add your redirect URL in the settings "http://xxxx/login.html"
* copy the client id to index.html
* cd into folder and run `python -m SimpleHTTPServer`

## Questions
* Do saved tracks not appear as playlist? -> yes they are separate.
* is the track order of a playlist exported correctly? -> yes

## Notes
* Songs without spotify id are usually local songs.

## Todo
* removed starred tracks, they are now just a playlist.
* update jquery version
* test import
* lint code
