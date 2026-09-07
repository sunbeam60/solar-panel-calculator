# Solar Panel Calculator

[Solar Panel Calculator - run it here](https://sunbeam60.github.io/solar-panel-calculator/)

A single-file web app for sizing a solar panel system. Pick a location on the map, set the panel tilt and direction, and see the estimated output, then test whether a battery keeps a load powered through the year and what the system saves against your tariff.

Open `index.html` in a browser. Everything runs client side; the page needs internet access for the map tiles, place search, the NASA POWER climate data and the two chart and map libraries loaded from CDNs.

## What it does

- **Location and orientation.** Leaflet map with street and satellite layers, a draggable pin, and an azimuth arrow you can line up with a roof. Tilt and direction can be set by sliders, by the compass and side-view graphics, or by clicking the tilt-by-direction heatmap.
- **Output model.** A clear-sky irradiance model (Meinel beam, Haurwitz global, isotropic diffuse and ground reflection) scaled month by month to NASA POWER's measured irradiance for the site. Shows annual and monthly output, a daily power profile for the best, average and worst day, and the optimal orientation.
- **System draw simulator.** Paint an hour-by-hour load in µW to GW, choose a battery from cell, portable, home and vehicle presets, and run an hourly year-long simulation of state of charge, outages and unused production.
- **Cost and return.** Hourly import and export price editors with UK tariff presets, standing charge, installed-cost defaults, optional cheap-hour grid charging, and monthly bill, payback, annualised return and cumulative cash-flow charts for solar only versus solar plus battery.
- **Share links.** The whole configuration is encoded in the URL, and a share button copies it.

## Notes

- Hours in the simulators are solar time.
- Prices and costs are whatever currency you choose; the tariff and installed-cost presets are UK figures, approximate for 2025.
- No battery degradation, replacement or export limit is modelled.
