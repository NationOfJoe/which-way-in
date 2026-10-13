# Which Way In

Checks how long it takes to get somewhere from home (RM14 2LX) three ways:

1. Public transport from home
2. Drive to Upminster station, then train
3. Drive to Gidea Park station, then train

Plus driving all the way, for comparison. You can plan by **leave at** or **arrive by**.

## Use it

- **In a browser:** open `web/index.html`.
- **On Android:** download `WhichWayIn.apk` from the [latest release](../../releases/tag/latest) and install it. You may need to allow installs from your browser or file manager.

Every push to `main` rebuilds the APK with GitHub Actions and replaces the latest release.

## Data sources

- Trains and buses: [TfL Journey Planner](https://api.tfl.gov.uk)
- Driving times: [OSRM](https://project-osrm.org) on OpenStreetMap (no live traffic, so a traffic allowance is added)
- Address search: [Photon](https://photon.komoot.io) and [postcodes.io](https://postcodes.io)

## Layout

- `web/index.html` — the whole app, one page
- `android/` — a small WebView wrapper that bundles the page into an APK
