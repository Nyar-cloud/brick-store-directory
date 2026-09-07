# Brick Store Directory

An open list of every LEGO® store we know of: **1003 stores** in **57 countries**, 993 of them open, 10 closed.

These are the raw files. The living version, with photos of every stamp, search, a map and the people collecting them, is at [brickstorestamps.com](https://brickstorestamps.com).

Last change **2026-09-07**. The list is rebuilt every Monday; [CHANGELOG.md](CHANGELOG.md) records what moved.

## What is in here

| File | Contents |
| --- | --- |
| [`data/stores.json`](data/stores.json) | All stores, one JSON array, the canonical form |
| [`data/stores.csv`](data/stores.csv) | The same list as CSV, ready for spreadsheets and My Maps |
| [`data/stores.geojson`](data/stores.geojson) | The 994 stores with coordinates, drawn as a map by GitHub itself |
| [`stores/`](stores/) | One readable page per country |
| [`stores/closed.md`](stores/closed.md) | Every store that has shut down, newest first |
| [`CHANGELOG.md`](CHANGELOG.md) | What changed, week by week |

## Stores by continent

| Continent | Stores |
| --- | --- |
| Europe | 212 |
| North America | 219 |
| Central America | 5 |
| South America | 46 |
| Asia | 461 |
| Asia/Europe | 14 |
| Africa | 7 |
| Oceania | 39 |

## Countries

| Country | Stores | Open | Closed |
| --- | --- | --- | --- |
| [Australia](stores/australia.md) | 33 | 31 | 2 |
| [Austria](stores/austria.md) | 2 | 2 | 0 |
| [Bahrain](stores/bahrain.md) | 1 | 1 | 0 |
| [Belgium](stores/belgium.md) | 3 | 3 | 0 |
| [Bosnia and Herzegovina](stores/bosnia-and-herzegovina.md) | 1 | 1 | 0 |
| [Brazil](stores/brazil.md) | 23 | 23 | 0 |
| [Bulgaria](stores/bulgaria.md) | 1 | 1 | 0 |
| [Canada](stores/canada.md) | 17 | 17 | 0 |
| [Chile](stores/chile.md) | 10 | 10 | 0 |
| [China](stores/china.md) | 247 | 247 | 0 |
| [Colombia](stores/colombia.md) | 8 | 8 | 0 |
| [Costa Rica](stores/costa-rica.md) | 3 | 3 | 0 |
| [Croatia](stores/croatia.md) | 1 | 1 | 0 |
| [Czechia](stores/czechia.md) | 2 | 2 | 0 |
| [Denmark](stores/denmark.md) | 10 | 10 | 0 |
| [France](stores/france.md) | 29 | 29 | 0 |
| [Germany](stores/germany.md) | 27 | 26 | 1 |
| [Greece](stores/greece.md) | 7 | 7 | 0 |
| [Hong Kong](stores/hong-kong.md) | 8 | 8 | 0 |
| [Hungary](stores/hungary.md) | 3 | 3 | 0 |
| [Iceland](stores/iceland.md) | 1 | 1 | 0 |
| [India](stores/india.md) | 5 | 5 | 0 |
| [Indonesia](stores/indonesia.md) | 26 | 26 | 0 |
| [Ireland](stores/ireland.md) | 2 | 2 | 0 |
| [Israel](stores/israel.md) | 11 | 11 | 0 |
| [Italy](stores/italy.md) | 36 | 36 | 0 |
| [Japan](stores/japan.md) | 44 | 44 | 0 |
| [Kazakhstan](stores/kazakhstan.md) | 1 | 1 | 0 |
| [Kuwait](stores/kuwait.md) | 2 | 2 | 0 |
| [Macau](stores/macau.md) | 1 | 1 | 0 |
| [Malaysia](stores/malaysia.md) | 27 | 27 | 0 |
| [Mexico](stores/mexico.md) | 36 | 36 | 0 |
| [Netherlands](stores/netherlands.md) | 6 | 6 | 0 |
| [New Zealand](stores/new-zealand.md) | 6 | 6 | 0 |
| [Panama](stores/panama.md) | 2 | 2 | 0 |
| [Peru](stores/peru.md) | 5 | 5 | 0 |
| [Philippines](stores/philippines.md) | 7 | 7 | 0 |
| [Poland](stores/poland.md) | 10 | 10 | 0 |
| [Portugal](stores/portugal.md) | 7 | 7 | 0 |
| [Qatar](stores/qatar.md) | 4 | 4 | 0 |
| [Romania](stores/romania.md) | 13 | 13 | 0 |
| [Saudi Arabia](stores/saudi-arabia.md) | 9 | 9 | 0 |
| [Serbia](stores/serbia.md) | 1 | 1 | 0 |
| [Singapore](stores/singapore.md) | 15 | 14 | 1 |
| [Slovenia](stores/slovenia.md) | 1 | 1 | 0 |
| [South Africa](stores/south-africa.md) | 7 | 7 | 0 |
| [South Korea](stores/south-korea.md) | 25 | 25 | 0 |
| [Spain](stores/spain.md) | 11 | 11 | 0 |
| [Sweden](stores/sweden.md) | 1 | 1 | 0 |
| [Switzerland](stores/switzerland.md) | 3 | 3 | 0 |
| [Taiwan](stores/taiwan.md) | 9 | 9 | 0 |
| [Thailand](stores/thailand.md) | 7 | 7 | 0 |
| [Turkey](stores/turkey.md) | 14 | 14 | 0 |
| [United Arab Emirates](stores/united-arab-emirates.md) | 11 | 11 | 0 |
| [United Kingdom](stores/united-kingdom.md) | 34 | 34 | 0 |
| [USA](stores/usa.md) | 166 | 160 | 6 |
| [Vietnam](stores/vietnam.md) | 1 | 1 | 0 |

## Fields

| Field | Meaning |
| --- | --- |
| `id` | Stable identifier, unchanged across updates |
| `name`, `name_local` | Store name, plus the local-script name where one exists |
| `type` | `official`, `popup` or `closed` |
| `closed`, `closed_year` | Whether the store is permanently closed, and the year it closed |
| `moved_to` | If the store moved, the id of the location that replaced it |
| `popup_from`, `popup_to` | Run of a temporary store (ISO dates) |
| `continent`, `country`, `city` | Location, in English |
| `address`, `address_local` | Street address, plus the local-script version where one exists |
| `latitude`, `longitude` | Coordinates. Some are city centres rather than the shop door |
| `phone` | Public phone number of the store |
| `services` | `bam`, `pab`, `minifigure_factory`, `mosaic_maker` |
| `url`, `country_url` | The store and its country on Brick Passport |
| `updated` | When the record was last edited |

Identifiers stay stable and fields are only ever added, never renamed or removed.
You can build on this file without watching for surprises.

## Where the data comes from

This directory is generated from [Brick Passport](https://brickstorestamps.com), a collection site for LEGO store stamps.
It is a one-way copy: the site is the source, this repository is the mirror, and it is rebuilt from scratch on every run.
Edits made here are overwritten, so please report corrections and new stores as an [issue](https://github.com/Nyar-cloud/brick-store-directory/issues/new/choose). See [CONTRIBUTING.md](CONTRIBUTING.md).

Coordinates are good enough to find the right town, not always the right doorway.
Closures are marked with the year where it is known.

## Licence

Data under [CC BY-SA 4.0](LICENSE), attribution to Brick Passport. The generator script lives in the Brick Passport repository.

## Not affiliated with the LEGO Group

LEGO® is a trademark of the LEGO Group, which does not sponsor, authorise or endorse this project.
This is a fan-made list compiled from public information.
