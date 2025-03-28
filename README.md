Worldwide Earthquakes API
============

Earthquake is a simple tool for getting earthquake data. It returns the earthquake data for the past hour.

![Build Status](https://img.shields.io/badge/build-passing-green)
![Code Climate](https://img.shields.io/badge/maintainability-B-purple)
![Prod Ready](https://img.shields.io/badge/production-ready-blue)

This is a Python API Wrapper for the [Worldwide Earthquakes API](https://apiverve.com/marketplace/api/earthquake)

---

## Installation
	pip install apiverve-worldwideearthquakes

---

## Configuration

Before using the earthquake API client, you have to setup your account and obtain your API Key.  
You can get it by signing up at [https://apiverve.com](https://apiverve.com)

---

## Usage

The Worldwide Earthquakes API documentation is found here: [https://docs.apiverve.com/api/earthquake](https://docs.apiverve.com/api/earthquake).  
You can find parameters, example responses, and status codes documented here.

### Setup

```
# Import the client module
from apiverve_worldwideearthquakes.apiClient import EarthquakeAPIClient

# Initialize the client with your APIVerve API key
api = EarthquakeAPIClient("[YOUR_API_KEY]")
```

---


### Perform Request
Using the API client, you can perform requests to the API.

###### Define Query

```
This API does not require a Query
```

###### Simple Request

```
# Make a request to the API
result = api.execute()

# Print the result
print(result)
```

###### Example Response

```
{
  "status": "ok",
  "error": null,
  "data": {
    "earthquakes_LastUpdated": 1740085202,
    "earthquakes_LastHour": 13,
    "earthquakes": [
      {
        "mag": 1.63,
        "place": "4 km SSW of Home Gardens, CA",
        "time": 1740084740320,
        "status": "automatic",
        "tsunami": 0,
        "sig": 41,
        "net": "ci",
        "types": ",nearby-cities,origin,phase-data,scitech-link,",
        "nst": 30,
        "dmin": 0.07665,
        "rms": 0.16,
        "gap": 212,
        "magType": "ml",
        "type": "earthquake",
        "title": "M 1.6 - 4 km SSW of Home Gardens, CA",
        "coordinates": [
          -117.5313333,
          33.8441667
        ]
      },
      {
        "mag": 1.53,
        "place": "3 km  of The Geysers, CA",
        "time": 1740084398050,
        "status": "automatic",
        "tsunami": 0,
        "sig": 36,
        "net": "nc",
        "types": ",focal-mechanism,nearby-cities,origin,phase-data,",
        "nst": 31,
        "dmin": 0.01013,
        "rms": 0.04,
        "gap": 61,
        "magType": "md",
        "type": "earthquake",
        "title": "M 1.5 - 3 km  of The Geysers, CA",
        "coordinates": [
          -122.770835876465,
          38.8066673278809
        ]
      },
      {
        "mag": 1.5,
        "place": "36 km SSW of Los Ybanez, Texas",
        "time": 1740083760065,
        "status": "automatic",
        "tsunami": 0,
        "sig": 35,
        "net": "tx",
        "types": ",origin,phase-data,",
        "nst": 21,
        "dmin": 0,
        "rms": 0.5,
        "gap": 98,
        "magType": "ml",
        "type": "earthquake",
        "title": "M 1.5 - 36 km SSW of Los Ybanez, Texas",
        "coordinates": [
          -102.118,
          32.437
        ]
      },
      {
        "mag": 1.28,
        "place": "2 km NNE of Rancho San Diego, CA",
        "time": 1740083416660,
        "status": "automatic",
        "tsunami": 0,
        "sig": 25,
        "net": "ci",
        "types": ",nearby-cities,origin,phase-data,scitech-link,",
        "nst": 18,
        "dmin": 0.02613,
        "rms": 0.18,
        "gap": 117,
        "magType": "ml",
        "type": "earthquake",
        "title": "M 1.3 - 2 km NNE of Rancho San Diego, CA",
        "coordinates": [
          -116.9288333,
          32.7591667
        ]
      },
      {
        "mag": 1.3,
        "place": "2 km N of The Geysers, CA",
        "time": 1740083145550,
        "status": "automatic",
        "tsunami": 0,
        "sig": 26,
        "net": "nc",
        "types": ",nearby-cities,origin,phase-data,",
        "nst": 17,
        "dmin": 0.008002,
        "rms": 0.02,
        "gap": 75,
        "magType": "md",
        "type": "earthquake",
        "title": "M 1.3 - 2 km N of The Geysers, CA",
        "coordinates": [
          -122.758499145508,
          38.792667388916
        ]
      },
      {
        "mag": 2.03,
        "place": "23 km NE of San Ardo, CA",
        "time": 1740083087170,
        "status": "automatic",
        "tsunami": 0,
        "sig": 63,
        "net": "nc",
        "types": ",nearby-cities,origin,phase-data,",
        "nst": 24,
        "dmin": 0.04482,
        "rms": 0.08,
        "gap": 78,
        "magType": "md",
        "type": "earthquake",
        "title": "M 2.0 - 23 km NE of San Ardo, CA",
        "coordinates": [
          -120.757835388184,
          36.1879997253418
        ]
      },
      {
        "mag": 1.5,
        "place": "18 km N of Nellis Air Force Base, Nevada",
        "time": 1740082632669,
        "status": "automatic",
        "tsunami": 0,
        "sig": 35,
        "net": "nn",
        "types": ",origin,phase-data,",
        "nst": 12,
        "dmin": 0.142,
        "rms": 0.352,
        "gap": 324.6699999999999,
        "magType": "ml",
        "type": "earthquake",
        "title": "M 1.5 - 18 km N of Nellis Air Force Base, Nevada",
        "coordinates": [
          -115.0204,
          36.4137
        ]
      },
      {
        "mag": 2.4,
        "place": "42 km ENE of Susitna North, Alaska",
        "time": 1740082487421,
        "status": "automatic",
        "tsunami": 0,
        "sig": 89,
        "net": "ak",
        "types": ",origin,phase-data,",
        "rms": 0.58,
        "magType": "ml",
        "type": "earthquake",
        "title": "M 2.4 - 42 km ENE of Susitna North, Alaska",
        "coordinates": [
          -149.1448,
          62.358
        ]
      },
      {
        "mag": 0.58,
        "place": "0 km  of The Geysers, CA",
        "time": 1740082396860,
        "status": "automatic",
        "tsunami": 0,
        "sig": 5,
        "net": "nc",
        "types": ",nearby-cities,origin,phase-data,",
        "nst": 8,
        "dmin": 0.01016,
        "rms": 0.04,
        "gap": 122,
        "magType": "md",
        "type": "earthquake",
        "title": "M 0.6 - 0 km  of The Geysers, CA",
        "coordinates": [
          -122.75666809082,
          38.7779998779297
        ]
      },
      {
        "mag": 0.77,
        "place": "4 km NNW of The Geysers, CA",
        "time": 1740082221410,
        "status": "automatic",
        "tsunami": 0,
        "sig": 9,
        "net": "nc",
        "types": ",nearby-cities,origin,phase-data,",
        "nst": 7,
        "dmin": 0.006593,
        "rms": 0.01,
        "gap": 141,
        "magType": "md",
        "type": "earthquake",
        "title": "M 0.8 - 4 km NNW of The Geysers, CA",
        "coordinates": [
          -122.78116607666,
          38.8066673278809
        ]
      },
      {
        "mag": 0.76,
        "place": "9 km NW of The Geysers, CA",
        "time": 1740082075350,
        "status": "automatic",
        "tsunami": 0,
        "sig": 9,
        "net": "nc",
        "types": ",nearby-cities,origin,phase-data,",
        "nst": 12,
        "dmin": 0.005851,
        "rms": 0.02,
        "gap": 80,
        "magType": "md",
        "type": "earthquake",
        "title": "M 0.8 - 9 km NW of The Geysers, CA",
        "coordinates": [
          -122.842498779297,
          38.8226661682129
        ]
      },
      {
        "mag": 1.8,
        "place": "47 km ENE of Susitna North, Alaska",
        "time": 1740081957855,
        "status": "automatic",
        "tsunami": 0,
        "sig": 50,
        "net": "ak",
        "types": ",origin,phase-data,",
        "rms": 0.79,
        "magType": "ml",
        "type": "earthquake",
        "title": "M 1.8 - 47 km ENE of Susitna North, Alaska",
        "coordinates": [
          -149.0437,
          62.3668
        ]
      },
      {
        "mag": 3.14,
        "place": "73 km N of Brenas, Puerto Rico",
        "time": 1740081663500,
        "status": "reviewed",
        "tsunami": 0,
        "sig": 152,
        "net": "pr",
        "types": ",origin,phase-data,",
        "nst": 10,
        "dmin": 0.8083,
        "rms": 0.23,
        "gap": 271,
        "magType": "md",
        "type": "earthquake",
        "title": "M 3.1 - 73 km N of Brenas, Puerto Rico",
        "coordinates": [
          -66.3835,
          19.1311666666667
        ]
      }
    ]
  },
  "code": 200
}
```

---

## Customer Support

Need any assistance? [Get in touch with Customer Support](https://apiverve.com/contact).

---

## Updates
Stay up to date by following [@apiverveHQ](https://twitter.com/apiverveHQ) on Twitter.

---

## Legal

All usage of the APIVerve website, API, and services is subject to the [APIVerve Terms of Service](https://apiverve.com/terms) and all legal documents and agreements.

---

## License
Licensed under the The MIT License (MIT)

Copyright (&copy;) 2025 APIVerve, and EvlarSoft LLC

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.