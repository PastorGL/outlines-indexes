This repo contains geospatial outlines and H3 indexes for some territories of interest.

Currently there are:
* US timezones, both standard and daylight

More to follow (i.e., individual US states).

H3 coverage is the most possible compact one (non-uniform) but unlike standard H3 'compact' coverage it doesn't have any holes between polygons. Any potential holes are always covered by polygons of highest resolution. Also selected range of index resolutions (7 to 10) guarantees the lowest possible number of polygons for any 'compact' coverage of territories in question considering said territory size.

It is delivered in TSV format, and fields are
1. index (H3 hex),
2. resolution,
3. offset from GMT,
4. and DST flag (boolean).

GeoJSON outlines have Features with Properties of tzid, daylight, and offset.
