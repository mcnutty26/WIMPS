# WIMPS: API

## General
* API endpoints should be located at music.lan/api
* All API endpoints should take data via POST unless otherwise specified

## Endpoints
### /add
* Accepts a file as ... HTTP multipart request?
* Returns status 200 on successful upload **and queue**, 403 on item limit reached, or 400 on other error
