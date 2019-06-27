<center>
<img align="left" src="cards/m00.jpg" height="120">
<h1>Tarot dataset</h1>
</center>

A json dataset of tarot cards, and corresponding scans of the [RWS deck][0].

`tarot-images.json` includes references to the scans, `tarot.json` does not.

## The cards
If you just want the scans for the cards, they're available as a [release][2].

The cards are acquired from [data.totl.net](http://data.totl.net/) via wget:
```sh
$ wget -r -np -nH --cut-dirs=3 -R index.html* -R *r.jpg -R *h.jpg http://data.totl.net/tarot-rwcs-images/
```
This command excludes cards in horizontal, reversed, and horizontal reversed positions.

The cards are all 350x600px, and are 7.37MB total.

## Copyright and license
The [Rider-Waite-Smith deck][0] is public domain in the US, [but not currently in the EU][1].

This project is available as open source under the terms of the [MIT License][MIT].

[0]: https://en.wikipedia.org/wiki/Rider-Waite_tarot_deck
[1]: https://en.wikipedia.org/wiki/Rider-Waite_tarot_deck#Copyright_status
[2]: https://github.com/equokka/tarot-json/releases/tag/v0
[MIT]: http://opensource.org/licenses/MIT
