# Mumbai in miniature

An original, no-backend South Mumbai map study. Pan/zoom, day/night, pause and follow a simulated taxi. 1,714 OSM building footprints and 1,171 road segments across Fort and Colaba. The landmark arch is a stylized original illustration, not a surveyed model.

## Run

The published repository is a self-contained `index.html` (data stored as gzip/base64 and unpacked with the browser DecompressionStream API). Open `index.html` in a browser. No install, build, account, API key or network request is needed. Alternatively: `python3 -m http.server 8000` then open localhost:8000.

## What this is not

Not live traffic, bus tracking, routing, a full Mumbai model or a replica of Small SF. Simulated vehicles loop on independent road polylines, with a left-hand lateral offset; intersections, signals, road connectivity, one-way restrictions and accurate collision avoidance are not modeled. The source extract omits one-way tags. Building heights mix mapped values and upstream estimates; some are capped at 80m for this stylized rendering. The ground grid is a graphic backdrop, not a mapped coastline. No live weather, aircraft or ships.

## Data and attribution

© OpenStreetMap contributors, ODbL 1.0: https://www.openstreetmap.org/copyright

The embedded map dataset in `index.html` is a bounded subset of the OSM-derived extract at https://github.com/jayprajapati009/mumbai-map/blob/main/data/city-data.json . That project's NOTICE states its OSM geometry snapshot was taken on 10 October 2026. The subset preserves the ODbL licence. Source center is 18.985° N, 72.835° E; local coordinates are metres in an equirectangular projection. Subset bounds are x -1550..750m, y -7700..-4700m. We reuse only the licensed map dataset, not that project's renderer or assets.

Concept inspiration: Small SF by Ari Dutilh, https://smallsf.com/about . Its code, images and video are not used here.

## License

MIT License

Copyright (c) 2026 Bhurva Sharma

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

This license does not cover data.js. That OpenStreetMap-derived database is licensed under the Open Database License 1.0: https://opendatacommons.org/licenses/odbl/1-0/ . © OpenStreetMap contributors. Data extraction credited in README.md.



Original renderer, UI and landmark art: MIT, see LICENSE. OSM-derived data: ODbL 1.0, separate from the renderer's code license.
