# MarkerMatch API

This documents how to use the Marker Match API.

A web client demo is provided here
[Web Demo](https://www.raydreams.com/Home/Color)

## API Key
You will need an API Key to query the API.

* **MatchColor** : Removes a quote from the CMS
	* Methods: GET|POST
	* inputs:
		* line (string) product line ID string
        * hex (string as hex color) color to match on
	* output: (list) top 9 matches
* **ProductLines** : Get the full list of product lines with their IDs
    * inputs: none
    * output: (list) list of all the product lines

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
