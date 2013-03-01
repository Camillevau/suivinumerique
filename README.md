# Suivi Numerique

Suivi Numerique is a couchapp for tracking visitors datas during physical events. Think forms, stored in CouchDB, run via Javascript and Sammy.js.

# !NOTE!

Unstable

## About

TODO

## Requirements

* A running CouchDB server (>= 0.11)
* [CouchApp](http://github.com/couchapp/couchapp) - You need the latest and greatest couchapp for the push to work without errors. Follow [these instructions](http://wiki.github.com/couchapp/couchapp/manual-2) to install from source

## Usage

All you need to do to get up and running after the requirements are installed is:

    $ couchapp push . http://localhost:5984/suivinumerique
    
It should print out instructions of where you can view it.

You can also set up a .couchapprc file that looks something like this:

    {
      "env": { 
        "default": {
          "db": "http://admin:password@localhost:5984/suivinumerique"
        }
      }
    }

Once that is set up you can just do:

    $ couchapp push


## Acknowledgments

Suivi Numerique is mainly based on Swinger (http://github.com/quirkey/swinger). 

### Technologies/Projects used

* [Sammy.js](http://code.quirkey.com/sammy) for frontend controller/routing
* [CouchApp](http://github.com/couchapp/couchapp) for hosting the app in CouchDB
* [Aristo CSS](http://github.com/maccman/aristo/tree/master) for base buttons/styles
* [Showdown](http://attacklab.net/showdown/) for Markdown
* [Prettify](http://code.google.com/p/google-code-prettify/) for Code higlighting
