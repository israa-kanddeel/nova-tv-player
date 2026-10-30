# NOVA TV trailer player

A one-page host for YouTube's official embedded player, used by the [NOVA TV](https://github.com/israa-kanddeel/nova-tv) app on LG webOS TVs.

YouTube's embed refuses to play inside apps that don't run from a web address (error 153), so the TV app opens this page — served by GitHub Pages — in a frame:

```
https://israa-kanddeel.github.io/nova-tv-player/?v=<YouTube video id>
```

The page only contains the YouTube player and a small `postMessage` bridge (play / pause / seek, and state updates back to the app). It holds no account data.
