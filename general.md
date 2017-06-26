# WIMPS: Setup

## Definitions
### Integrated and decoupled music servers
* Integrated music servers expose an API and serve web pages
* Decoupled music servers are those which only expose an API
### Entries
* Entries represent media which has been sent to the server
* Entries are JSON objects with an `id` field (the unique identifier for the user who owns the entry) and a `name` field (the title of the entry)

## General
* Music servers must work when accessed at http://music.lan
* Each user must be uniquely identifiable (IP addresses or account usernames are common identifiers)

## Compatibility
* Music servers must run on Debian 8.7
* For music servers which use an interpreter or virtual machine (e.g. python or Java), they must run on the version of that software which is in the Debian stable repository
* For decoupled music servers which use a scripting language in their web pages, they must run on the version of that software which is in the Debian stable repository

## Queuing
* The server must store enough information on items queued by users to play them (this need not be a file, e.g. a URL for a youtube video)
* The order in which items are submitted to the server must be stored
* The user who submitted an item to the server must be stored

## Playing Media
* MPV must be used to play items, and invoked using `mpv` (rather than using an absolute path)
* Media must be volume normalised when playing
* There must be a limit on the amount of time that an item can play

## Ports
* Decoupled music servers must expose their API on port 8080
* Integrated music servers must expose their API on port 80
