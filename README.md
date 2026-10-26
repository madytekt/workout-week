# workout-week

A one-page schedule of the next 7 days of classes at two Somerville studios, side by side:

- **EMBODI Studios** (11 Bow St): Pilates, Strength, Yoga, Turn Up
- **F45 Training East Somerville** (442 McGrath Hwy)

Live site: https://madytekt.github.io/workout-week/

## How it works

`index.html` is the whole site. When you open it, your browser pulls the schedule straight from each studio's booking system:

- EMBODI: the Arketa schedule feed behind embodistudios.com/schedule
- F45: F45's booking API for studio 4563

Nothing runs on a server and nothing is stored here. The page caches results in your browser for 30 minutes; the Refresh button fetches again.

Each class shows time, workout, trainer, and spots left (red at 3 or fewer). Past classes are greyed out.

## If it breaks

Both feeds are public but undocumented, so a studio changing its booking system can break its column. The page shows an error with a link to the studio's own schedule when that happens.
