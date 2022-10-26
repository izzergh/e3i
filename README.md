```
      ____  _
     |___ \(_)             (_)
  ___  __) |_    __ _ _ __  _
 / _ \|__ <| |  / _` | '_ \| |
|  __/___) | | | (_| | |_) | |
 \___|____/|_|  \__,_| .__/|_|
                     | |
                     |_|
```

This is the source code for e3i, an emoji API.
The goal of this API is to support the following:

- return the literal character or character sequence in an emoji query
- search in both directions (i.e. search by an emoji or search by name)
- browse indexes
- all the aliases and languages in the [Unicode CLDR](https://cldr.unicode.org/)
- search proprietary sets, like those used by GitHub and Slack (as long as
  they correspond to Unicode characters - not planning on sending images)

There are other APIs that do some subset of these, and there are other APIs
  that have features not in the above list.

<!-- TODO: link to some of these for completion's sake -->

## Roadmap

In no particular order (but probably the first one first!):

- [ ] Set up skeleton app
- [ ] Add a rake task for pulling CLDR JSON data (use a git sub-module?)
- [ ] Add search-by-name for non-CLDR Unicode named emoji, and specs
- [ ] Add search-by-name for CLDR named emoji for English, and specs
- [ ] Add search-by-name for CLDR named emoji for other languages (specs?)
- [ ] Add search-by-emoji for single-character emoji, and specs
- [ ] Add search-by-emoji for multiple-character emoji, and specs
- [ ] Add emoji index endpoint, and specs
- [ ] Determine hosting for a sample app
- [ ] Document deploying the API to one's own server
- [ ] Document setting up the API locally for development
- [ ] Add search-by-name and search-by-emoji for Slack
- [ ] ditto, for GitHub
- [ ] ditto, for Discord
