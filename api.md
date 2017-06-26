# WIMPS: API

## General
* API endpoints should be located at music.lan/api
* All API endpoints should take data via POST unless otherwise specified
* All API endpoints should return 200 on receipt of a valid request, and 400 on other error, unless otherwise specified

## Entries
* Whenever it is specified that an entry is returned, that entry takes the form of a JSON Object with the following fields:
  * 'id': The unique identifier for the user who owns the entry
  * 'name': The title of the entry

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
