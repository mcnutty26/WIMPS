# WIMPS: General Setup

## Misc
* Music servers must work when accessed at http://music.lan
* Each user must be uniquely identifiable (IP addresses or account usernames are common identifiers)

## Queuing
* The server must store enough information on items queued by users to play them (this need not be a file, e.g. a URL for a youtube video)
* The order in which items are submitted to the server must be stored
* The user who submitted an item to the server must be stored

## Playing Media
* MPV must be used to play items, and invoked using `mpv` (rather than using an absolute path)
* Media must be volume normalised when playing
* There must be a limit on the amount of time that an item can play
