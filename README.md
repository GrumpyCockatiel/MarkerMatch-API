# MarkerMatch API

This documents how to use the Marker Match API.

A web client demo is provided here
[Web Demo](https://www.raydreams.com/Home/Color)

## Endpoint

The base endpoint is:

`https://tagio.app/api/<function_name>`

## API Key
You will need your own assigned API Key to query the API.

Please use the contact form at

[Contact Form](https://www.raydreams.com/Home/Contact)

to request your own API key.

## Methods

* **MatchColor** : Matches the specified color against all the markers in the product for the top matches. Either RGB or Hex is required where RGN takes precedence.
	* Methods: GET|POST
	* inputs:
		* line (string) product line ID string
        * rgb (string as an RGB tuple) color to match on. e.g. `101,45,90`
        * hex (string as hex color) color to match on, preceedint # is optional
	* output: (list) top 9 matches
* **ProductLines** : Get the full list of product lines with their IDs
    * Methods: GET
    * inputs: none
    * output: (list) list of all the product lines

## Request Header

Requests should only sent over HTTPS using TLS 1.2.

```
Content-Type:application/json
x-api-authorization:<your_api_key>
x-timestamp:<ISO 8601 DateTime string with TimeZone>
```

## Response

All responses are currently in JSON wrapped in a response object with the format:

```
{
    "resultType": "Success",
    "result": <json_object>,
    "isSuccess": true
}

```

Result contains the data object queried.

## Security

Requests are currently throttled to limit only so many requets in a 24 hour period for a specific key.

Signing is not yet implemented but is coming.

## Bugs and Issues

You can report bugs and issues here.

## Current Vendor List

1. Copic Sketch
2. Copic Ciao
3. Copic Classic
4. Copic Wide
5. Prismacolor Premier Chisel
6. Prismacolor Premier Brush
7. Prismacolor Premier Softcore
8. Faber-Castell Polychromos
9. Spectrum Noir Markers
10. Touch Twin Markers
11. Touch Twin Brush Markers
12. Tombrow Brush Markers
13. Letraset Tria
14. Winsor & Newton BrushMarker
15. Winsor & Newton ProMarker
16. Blick Brush Markers
17. Zig Brush Markers

Ohuhu is currently being added and coming soon.