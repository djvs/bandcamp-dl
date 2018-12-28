### bandcamp-dl

Wrapper around `youtube-dl` for yanking an artist's discography off of Bandcamp.

Usage: 
```
bandcamp-dl https://someartist.bandcamp.com/album/whatever
```

Will automatically search for links to an artist's discography page and then download each album individually, prefixing the album's name with an artist's name on multi-artist discography pages.  

## Requirements

* youtube-dl
* A recent version of ruby
* Ruby gems:
  * curb
  * nokogiri
  * pry

Will automatically dump you in a pry-console after album discovery after showing you a quick manifest of the albums it wants to download.  Press Ctrl-D or type `exit` to continue, or `exit-program` to abandon ship.

Please use responsibly and support artists you think deserve it!
