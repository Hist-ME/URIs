# ISMI Non-aligned Place URIs
These are places that have not yet been successfully aligned with external authorities. 

Jump to [Source Project](#source-project) | [Version](#version) | [File Format](#file-format)

## Source Project
### Islamic Scientific Manuscript Initiative database [ISMI](https://ismi.mpiwg-berlin.mpg.de)

These are places from the ISMI database of manuscripts. These places are in some way related to manuscripts, either directly as the place a manuscript was copied or a text was created or as the current location of the manuscript's holding library or more indirectly like the place an author or copyist was born, lived in or died.

## Version

### 0.5

Updated list containing only places with references and a short description of the kind of references the database contains to the place.

### 0.0.1

Very first version of place list.

## File Format

### ismi-places.tsv

| field | description |
| --- | --- |
| id  | ISMI database ID |
| title | place name in ISMI database |
| variants | other names for this place in ISMI database |
| types  | ISMI place type |
| title_source  | URI in ISMI database web frontend |
| title_uri  | URI in ISMI database web frontend |
| parent_name | name of parent place in ISMI db |
| parent_id  | id of parent place in ISMI db |
| start | dummy start date (800CE) |
| attestation_year | dummy attestation date (2016CE) |
| description | compact description of the relations to this place in the ISMI db |

Also see [the general README](https://github.com/Hist-ME/URIs/blob/master/README.md) for this repo.