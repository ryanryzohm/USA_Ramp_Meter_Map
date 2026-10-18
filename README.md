# North American Ramp Meter Inventory

The **North American Ramp Meter Inventory** is an open geospatial dataset of ramp-meter locations across the United States and the Toronto metropolitan area of Canada.

**Version 1.0 contains 5,351 individually mapped ramp-meter locations** across dozens of metropolitan areas.

The goal of this project is to create a freely available, centralized inventory of ramp-meter infrastructure that can be used for transportation research, visualization, geographic comparison, and other applications.

Created and maintained by **Ryan Wang ([@ryanryzohm](https://github.com/ryanryzohm))**.

## Map

The original inventory was created in **Google My Maps**, with individual markers placed at identified ramp-meter locations.

The dataset includes systems ranging from small pilot installations with only a few meters to large regional networks containing hundreds or more than one thousand locations.

Major concentrations include California and the Minneapolis–Saint Paul region, along with substantial systems in several other metropolitan areas.

## Data

This repository includes:

- **CSV** — 5,351 ramp-meter locations in a single table
- **KML** — geographic data exported from the original Google My Maps project

Coordinates use **WGS 84 (EPSG:4326)**.

The CSV currently contains the following fields:

- `state_group` — regional/state grouping used in the original map
- `X` — longitude
- `Y` — latitude
- `Z` — altitude
- `Name` — ramp or location name
- `description` — optional descriptive information

## Methodology

Ramp-meter systems were first identified using a combination of transportation-agency publications, DOT reports and studies, project announcements, news articles, web searches, and existing regional summaries.

These sources were primarily used to determine **which metropolitan areas and freeway corridors were known to have ramp-metering systems**.

The majority of individual ramp-meter locations in the dataset were then identified through **manual visual inspection of satellite imagery**.

A common visual indicator was the transverse white stop line located across a freeway entrance ramp near the ramp-meter signal. Freeway corridors within known ramp-metering regions were manually scanned for these features.

When a location was unclear from satellite imagery alone, **Google Street View was used for additional visual verification**, including checking for ramp-meter signal heads, stop lines, signage, lane configuration, and other associated infrastructure.

For smaller systems or newly installed projects, transportation-agency documents and news reports sometimes identified the specific ramps or corridors directly. For large systems containing hundreds of meters, manual satellite-image inspection was the primary method used to identify individual locations.

The dataset therefore represents a manually assembled geospatial inventory combining:

- transportation-agency reports and publications;
- DOT studies and ramp-meter project documents;
- installation announcements and news reports;
- web-based research identifying known ramp-meter systems;
- manual inspection of satellite imagery; and
- street-level visual verification where needed.

The mapping process was conducted manually rather than through automated image recognition.

## Coverage and Limitations

This dataset is intended to provide broad geographic coverage but should **not yet be interpreted as a guaranteed complete inventory of every ramp meter in North America**.

Coverage varies between regions. Some metropolitan systems have been mapped extensively, while others may contain only known projects, pilots, or locations identified through available documentation.

Possible limitations include:

- missing installations;
- historical or decommissioned ramp meters;
- changes in operating status after a location was mapped;
- ambiguous locations requiring further verification;
- uneven coverage between metropolitan areas;
- differences in the availability and age of satellite and street-level imagery.

Absence of a mapped ramp meter does not necessarily indicate that no ramp meter exists at that location.

Future versions of the dataset will include additional validation against transportation-agency inventories where authoritative point-level or corridor-level data are available.

Corrections, additions, supporting sources, and other contributions are welcome.

## Validation

The dataset has been manually assembled from multiple independent sources and visual observations.

Formal validation against authoritative transportation-agency inventories is planned for selected metropolitan areas where sufficiently detailed agency data are publicly available.

Validation efforts may include:

- comparison between mapped locations and agency inventories;
- random sampling of mapped locations for independent verification;
- measurement of confirmed
