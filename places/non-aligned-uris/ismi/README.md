# ISMI Non-aligned Place URIs
These are places that have not yet been successfully aligned with external authorities. 

Jump to [Source Project](#source-project) | [Version](#version) | [File Format](#file-format)

## Source Project
### Islamic Scientific Manuscript Initiative database [ISMI](https://ismi.mpiwg-berlin.mpg.de)

These are places from the ISMI database of manuscripts. These places are in some way related to manuscripts, either directly as the place a manuscript was copied or a text was created or as the current location of the manuscript's holding library or more indirectly like the place an author or copyist was born, lived in or died.

## Version

### 0.0.1

Very first version of place list.

## File Format

### ismi-places.tsv

| field | description |
| --- | --- |
| uri | URI in ISMI database web frontend |
| description | place name in ISMI database |
| id | ISMI database ID |
| type | ISMI place type |
| parent_name | name of parent place in ISMI db |
| parent_id | ID of parent place in ISMI db |
| parent_type | type of parent place in ISMI db |

### ismi-places-lp.tsv

Linked Places TSV (LP-TSV) v0.2 format (see [LP-TSV documentation](https://github.com/LinkedPasts/linked-places/blob/master/tsv_0.2.md))

| field | description |
| --- | --- |
| id | ISMI database ID |
| title | place name in ISMI database |
| title_uri | URI in ISMI database web frontend |
| title_source | "ISMI" |
| start | dummy attestation date (700CE) |

Also see [the general README](https://github.com/Hist-ME/URIs/blob/master/README.md) for this repo.