# realtime-tracker
Track the International Space Station in real time as it revolves around the earth at 17,500 mph

## How to Run

1. Download the repository or clone it to your local machine
2. Obtain a MapBox access token from [this page](https://docs.mapbox.com/help/glossary/access-token/)
3. Edit [mapanimation.js](./mapanimation.js), and replace `ADD-YOUR-MAPBOX-ACCESS-TOKEN-HERE` with your MapBox access token.
4. Open [index.html](./index.html)
5. Click on the `Show live ISS Location` button
6. The ISS icon should now start moving across the map at constant intervals. You can pan and zoom in and out of the map, but ISS always centers itself. Hover on the icon to see the current latitude and longitude.
7. Sometimes MapBox may not be responsive and the ISS icon may not start moving immediately. Click on the `Show live ISS Location` button again, and this should address the problem.

## Roadmap of future improvements

- In case ISS does not start moving automatically (likely because of MapBox rate limits), constrain the request rate and call the API again until it starts moving across the map.
- Track other satellites that are orbiting the earth and have APIs we can access.
- Embed the [ISS live view feed video](https://eol.jsc.nasa.gov/ESRS/HDEV/) in the map.
- Notify the user when ISS is close to their location.

## License information

This project is licensed using an `MIT License`. For more information on the license, refer to this [file](./LICENSE).
