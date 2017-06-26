# WIMPS: API

## Definitions
Please see [Setup](https://github.com/mcnutty26/WIMPS/blob/master/general.md)

## General
* API endpoints must be located at music.lan/api
* All API endpoints must take data via POST unless otherwise specified
* All API endpoints must return 200 on receipt of a valid request, and 400 on other error, unless otherwise specified

## Endpoints
### /add
* Accepts a file as ... HTTP multipart request?
* Returns status 200 on successful upload **and queue**.
### /url
* Accepts a URL as a string with the variable name 'url'.
* Returns status 200 on receipt of a valid reuqest, which does not include downloading the entry.
### /current
* Returns the current entry.
### /queue
* Returns a JSON object containing a list of entries in the music server queue.
* This does **not** include the currently playing entry.
