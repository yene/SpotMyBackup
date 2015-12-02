# SpotMyBackup
Backup and Restore your Spotify Playlists and "My Music".

This javascript based app allows you to backup all your playlists and import them in any other Spotify Account. It uses the OAuth-Functionality of Spotify to be able to handle your personal playlists. 

In consequence, no credentials or data is stored or processed on the Webserver itself.

You can use it at http://spotify.yannickweiss.com/ or on your own webserver (see Setup).

## Documentation
* [Spotify Web API](https://developer.spotify.com/web-api/endpoint-reference/)

## Setup
* Create new app https://developer.spotify.com/my-applications
* Add your redirect URL in the settings "http://xxxx/login.html"
* If you get `INVALID_CLIENT: Invalid redirect URI` see previous step.
* Copy the client id to index.html
* `cd` into folder and run `python -m SimpleHTTPServer`

## Questions
* Do saved tracks not appear as playlist? -> yes they are separate.
* is the track order of a playlist exported correctly? -> yes

## Notes
* Songs without spotify id are usually local songs.

## Todo
* removed starred tracks, they are now just a playlist.
* Update jquery version and remove dependency.
* test import
* lint code
* give credit to first version "based on ..."
* Add security information that login information are not sent to any server, link to app.js.
