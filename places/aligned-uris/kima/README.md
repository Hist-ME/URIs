# KIMA aligned Place URIs
Place that have been successfully aligned with external authorities. 

Jump to [Source Project](#source-project) | [Version](#version) | [File Format](#file-format) | [Fields](#fields) | [Warnings/Quirks](#warningsquirks)

## Source Project
### [http://data.geo-kima.org/](http://data.geo-kima.org/)
Kima historical gazetteer is based mainly on the authority files of the National Library of Israel, which records over 27000 places with their English and Hebrew preferred names, as well as additional variants. With addition of attested Hebrew variants from the Library cataogue as well as from annotated sources. The data is currently mostly print-era data, but slowly earlier attestations and variants are also integrated. The data is available at the Kima website both through a user interface,  through an API and also on Recogito's annotation platform. An open refine plugin for reconciliation is available [here](https://github.com/embaral/KIMA-reconciliation). 

## Version
### [version number]
[link to versioned data source (if applicable), comments about any post-processing]

## File Format
The records which are already aligned with Wikidata or Geonames and have coordinate information are available as Linked Places TSV (LP-TSV) v0.2 (see [LP-TSV documentation](https://github.com/LinkedPasts/linked-places/blob/master/tsv_0.2.md)).

### Fields
Here is how we use the LP-TSV fields.
| field | description |
| --- | --- |
| id |  |
| title |  |
| description |  |
| variants |  |
| types |  |
| matches |  |
| start |  |
| title_source |  |
| title_uri | |

The records which are aligned only with VIAF records do not yet have coordinates are available as tsv with the following fields:

### Fields
Here is how we use the LP-TSV fields.
| field | description |
| --- | --- |
| id |  |
| title |  |
| description |  |
| variants |  |
| types |  |
| matches |  |
| start |  |
| title_source |  |
| title_uri | |
Finally, alignments of KIMA with Usaybie


## Warnings/Quirks
- [list of warnings/quirks/NB items for your dataset] 




Also see [the general README](https://github.com/Hist-ME/URIs/blob/master/README.md) for this repo.
