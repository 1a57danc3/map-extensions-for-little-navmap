![](https://cdn.via.moe/file/viamoe/img/lnm-tool.jpg)

This repo includes many custom maps for Little Navmap 2.8.x :

* Google Maps (Default)
* Google Maps (Satellite)
* Google Maps (Terrain)
* Mapbox Streets
* Mapbox Outdoors
* Mapbox Light
* Mapbox Dark
* Mapbox Satellite
* Mapbox Satellite Streets
* Mapbox Navigation Day
* Mapbox Navigation Night
* U.S. VFR Sectionals
* U.S. IFR Enroute Low
* U.S. IFR Enroute High
* U.S. IFR Area Charts
* U.S. Terminal Area Charts (TAC)
* U.S. Helicopter Route Charts
* Norway Topographic Maps
* Sweden Topographic Maps
* Finland Topographic Maps
* Open Street Maps
* Open Flight Maps
* Arcgis
* IGN Géoservices

To use the maps:

1. make sure Little Navmap is closed.

2. drop the 'data' folder inside the zip-file into the root Little Navmap folder, overwrite when asked.

3. run Little Navmap and select one of the above maps from the drop-down menu 'Select map theme' located at the top right corner above the Map window.

Enjoy! 

------

# Credit

https://www.avsim.com/forums/topic/548994-new-maps-for-lnm/

https://flightsim.to/file/6411/map-extensions-for-little-navmap-lnm

https://flightsim.to/file/13899/littlenavmapofmtheme

https://www.bilibili.com/video/BV1xP4y1A7Ky

https://github.com/albar965/littlenavmap/issues/479#issuecomment-1117965128

https://docs.mapbox.com/api/maps/styles/

-----

Thanks for `Cloudflare worker`

Porxy Script:

```
addEventListener(
	"fetch",event => {
		let url=new URL(event.request.url);
		url.hostname="tiles.satellite.image";
		let request=new Request(url,event.request);
		event. respondWith(
			fetch(request)
		)
	}
)
```

Some maps preview in [Viamap](https://maps.via.moe/)
