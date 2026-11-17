# openbot-weather-backdrop

Live: https://sunnyegg.github.io/openbot-weather-backdrop/ - the weather updates itself.

Bahasa / Language: [Indonesia](README.md) | **English**

A living landscape with live Jakarta weather, made as an OpenBot backdrop.

- The sky shifts with the local WIB (UTC+7) clock, from dawn to night
- Jakarta weather (cloud cover, rain, storms) from [open-meteo](https://open-meteo.com/), refreshed every 10 minutes
- Built-in weather snapshot, used when the fetch fails
- Canvas: drifting clouds + rain + lightning
- Three hill layers, sun/moon, stars, and a horizon haze

## Usage

Open `index.html` directly in a browser, or set it as an OpenBot backdrop:

1. Pass the contents of `index.html` as the `html` argument of `openbot.set_backdrop`
2. `title`: whatever name you want
3. `bubbles`: bubble colors, e.g. `{ "yours": "#33526e", "agents": "#1f3040" }`

## Change the location

Edit the two constants at the top of the `<script>` in `index.html`:

```js
var LAT = '-6.2088', LON = '106.8456'; // Monas, Jakarta
```

Swap in coordinates for another city, e.g. Bandung `-6.9175, 107.6191`.

One file, no dependencies, no build. Just open it.
