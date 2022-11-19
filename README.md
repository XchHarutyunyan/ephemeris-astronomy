### Installation

`npm install ephemeris-astronomy`

### Usage

*app.js*
```javascript
const ephemerisAstronomy = require('ephemeris-astronomy');
const dateObj = new Date('2022-11-20T01:18:12.000+04:00');

// parameters: ephemerisAstronomy.getAllPlanets(dateObj, longitude, latitude, height);
var result = ephemerisAstronomy.getAllPlanets(dateObj, 10.0014, 53.5653, 0);

/* Check out the namespaces: date, observer and observed:

{
  "date": {
    "gregorianTerrestrial": "19.11.2022 21:18:47",
    "gregorianTerrestrialRaw": {
      "day": 19,
      "month": 11,
      "year": 2022,
      "hours": 21,
      "minutes": 18,
      "seconds": 47,
      "julianDate": 2459902.5,
      "julianTime": 0.8880439814814814,
      "julian": 2459903.3880439815,
      "j2000": 2022.8840192853704,
      "b1950": 2022.884230099881,
      "j1900": 2022.8840192853704,
      "delta": 73.26395876416308,
      "terrestrial": 2459903.3880439815,
      "universal": 2459903.387196019,
      "universalDate": {
        "julian": 2459903.387196019,
        "year": 2022,
        "month": 11,
        "day": 19,
        "hours": 21,
        "minutes": 17,
        "seconds": 33,
        "milliseconds": 736
      },
      "universalDateString": "19.11.2022 21:17:33.736"
    },
    "gregorianUniversal": "19.11.2022 21:17:33.736",
    "gregorianDelta": "00:00:73.26395876416308",
    "julianTerrestrial": 2459903.3880439815,
    "julianUniversal": 2459903.387196019,
    "julianDelta": 0.000847962485696332
  },
  "observer": {
    "name": "earth",
    "longitudeGeodetic": "",
    "longitudeGeocentric": "",
    "latitudeGeodetic": "",
    "latitudeGeocentric": 0,
    "heightGeodetic": 0,
    "heightGeocentric": 6378.137
  },
  "observed": {
    "sun": {
      "name": "sun",
      "raw": [Object],
      "apparentLongitudeDms30": "27°30'55\"",
      "apparentLongitudeDms360": "237°30'55\"",
      "apparentLongitudeDd": 237.515368175618,
      "geocentricDistanceKm": -1
    },
    "mercury": {
      "name": "mercury",
      "raw": [Object],
      "apparentLongitudeDms30": "3°56'26\"",
      "apparentLongitudeDms360": "243°56'26\"",
      "apparentLongitudeDd": 243.9407643564857,
      "geocentricDistanceKm": -1
    },
    "venus": {
      "name": "venus",
      "raw": [Object],
      "apparentLongitudeDms30": "4°33'23\"",
      "apparentLongitudeDms360": "244°33'23\"",
      "apparentLongitudeDd": 244.55653526303124,
      "geocentricDistanceKm": -1
    },
    "moon": {
      "name": "moon",
      "raw": [Object],
      "apparentLongitudeDms30": "5°33'10\"",
      "apparentLongitudeDms360": "185°33'10\"",
      "apparentLongitudeDd": 185.5528776124193,
      "geocentricDistanceKm": 60.5984314321428
    },
    "mars": {
      "name": "mars",
      "raw": [Object],
      "apparentLongitudeDms30": "22°38'9\"",
      "apparentLongitudeDms360": "82°38'9\"",
      "apparentLongitudeDd": 82.63599890916993,
      "geocentricDistanceKm": -1
    },
    "jupiter": {
      "name": "jupiter",
      "raw": [Object],
      "apparentLongitudeDms30": "28°49'40\"",
      "apparentLongitudeDms360": "358°49'40\"",
      "apparentLongitudeDd": 358.8278914748483,
      "geocentricDistanceKm": -1
    },
    "saturn": {
      "name": "saturn",
      "raw": [Object],
      "apparentLongitudeDms30": "19°14'27\"",
      "apparentLongitudeDms360": "319°14'27\"",
      "apparentLongitudeDd": 319.2410891295679,
      "geocentricDistanceKm": -1
    },
    "uranus": {
      "name": "uranus",
      "raw": [Object],
      "apparentLongitudeDms30": "16°28'36\"",
      "apparentLongitudeDms360": "46°28'36\"",
      "apparentLongitudeDd": 46.476905951692125,
      "geocentricDistanceKm": -1
    },
    "neptune": {
      "name": "neptune",
      "raw": [Object],
      "apparentLongitudeDms30": "22°42'4\"",
      "apparentLongitudeDms360": "352°42'4\"",
      "apparentLongitudeDd": 352.70138074063647,
      "geocentricDistanceKm": -1
    },
    "pluto": {
      "name": "pluto",
      "raw": [Object],
      "apparentLongitudeDms30": "26°32'22\"",
      "apparentLongitudeDms360": "296°32'22\"",
      "apparentLongitudeDd": 296.53971382673024,
      "geocentricDistanceKm": -1
    },
    "chiron": {
      "name": "chiron",
      "raw": [Object],
      "apparentLongitudeDms30": "12°32'52\"",
      "apparentLongitudeDms360": "12°32'52\"",
      "apparentLongitudeDd": 12.548049105841285,
      "geocentricDistanceKm": -1
    },
    "sirius": {
      "name": "sirius",
      "raw": [Object],
      "apparentLongitudeDms30": "11°32'25\"",
      "apparentLongitudeDms360": "101°32'25\"",
      "apparentLongitudeDd": 1.7722157109576746,
      "geocentricDistanceKm": 7777
    }
  }
}
*/
```
### Contributors

This implementation based on code by [Steve Moshier](http://www.moshier.net).


### License

[GPLv3](https://www.gnu.org/licenses/gpl-3.0.html)
