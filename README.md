## bandcamp-dl

Wrapper around `youtube-dl` for yanking an artist's discography off of Bandcamp.

Will automatically search for links to an artist's discography page and then download each album individually, prefixing the album's name with an artist's name on multi-artist discography pages.  

Please use responsibly and support artists you think deserve it!

### Requirements

* youtube-dl
* A semi-recent version of Ruby (honestly it probably even works with Ruby v1.9.2 or so, haven't tested it tho)
* Ruby gems:
  * curb
  * nokogiri
  * pry


### Installation
```
cd /tmp
wget https://github.com/djvs/bandcamp-dl/blob/master/bandcamp-dl
sudo cp bandcamp-dl /usr/bin/
sudo chmod +x /usr/bin/bandcamp-dl
```

### Usage

```
bandcamp-dl https://someartist.bandcamp.com/album/whatever
```

Will automatically dump you in a pry-console after album discovery after showing you a quick manifest of the albums it wants to download.  Press Ctrl-D or type `exit` to continue, or `exit-program` to abandon ship.

