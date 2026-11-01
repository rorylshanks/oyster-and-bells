# Oyster & Bells

A cosy, Animal Crossing-flavoured live departures board for any two London Underground stations. Made for a tablet in landscape, and happy on anything else with a browser.

**[Open it](https://rorylshanks.github.io/oyster-and-bells/)**, choose two stations, and bookmark the page that opens.

## Choosing stations

Stations live in the URL, so the board keeps no settings of its own:

```
https://rorylshanks.github.io/oyster-and-bells/?stations=940GZZLUBNK,940GZZLUOXC
```

That's Bank and Oxford Circus. The IDs are TfL NaPTAN codes, and the picker fills them in for you. Leave out `stations` to get the picker.

## Good to know

- Times refresh every 30 seconds and count down in between.
- Trains that terminate at the station are hidden, since you can't board them. Trains that start or reverse there only appear once TfL lists them with a destination, which is often when they reach the platform. At a terminus, that means short notice.
- To keep a tablet awake, the page asks the browser to hold the screen on. If yours doesn't, extend the screen timeout in its settings.

It's one HTML file with no build step and no backend. The browser talks straight to the TfL API, and no API key is needed.

Powered by TfL Open Data.
