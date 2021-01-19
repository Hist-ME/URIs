# Usaybia.net Non-aligned Place URIs
These are places that have not yet been successfully aligned with external authorities. 

Jump to [Source Project](#source-project) | [Version](#version) | [File Format](#file-format) | [Fields](#fields) | [Warnings/Quirks](#warningsquirks)

## Source Project
### [The Communities of Knowledge (Usaybia.net Project)](https://usaybia.net)

The places here are based on those in the the usaybia.net dataset, which consists primarily of TEI-XML records and can be found in the [usaybia/usaybia-data](https://github.com/usaybia/usaybia-data/) repo. The dataset is also available as raw data from individual records at the [usaybia.net](https://usaybia.net) website or as an [archive package in Zenodo](https://zenodo.org/record/3975506) ([DOI: 10.5281/zenodo.3975505](https://doi.org/10.5281/zenodo.3975505)).

The initial identification of places was based on the index of Emilie Savage-Smith, Simon Swain, and G. J. H. van Gelder, eds., _A Literary History of Medicine: The “Uyūn al-anbā” fī ṭabaqāt al-aṭibbā’ of Ibn Abī Uṣaybi’ah_, 5 vols. (Leiden: Brill, 2020), https://dh.brill.com/scholarlyeditions/library/urn:cts:arabicLit:0668IbnAbiUsaibia/.

Other place records from or related to Ibn Abī Uṣaybiʿa's text are added as relevant for the project's analysis.

## Version
### v0.4-beta
Records here are processed from [v0.4-beta](https://github.com/usaybia/usaybia-data/releases/tag/v0.4-beta) of the data available at the usaybia/usaybia-data repo.

However, while processing this data we may have deduplicated or disambiguated records in ways not yet reflected in the source repo.

## File Format
Linked Places TSV (LP-TSV) v0.2 (see [LP-TSV documentation](https://github.com/LinkedPasts/linked-places/blob/master/tsv_0.2.md))

## Fields
Here is how we use the LP-TSV fields.
| field | description |
| --- | --- |
| id | usaybia.net place URI |
| title | romanized name of the place as found in the LHOM translation |
| description | short description of the place, copied or slightly adapted from the LHOM index when it is provided there |
| variants | alternate names for the place, usually romanizations from the LHOM index, but possibly also names in Arabic or other non-Latin scripts added by the usaybia.net team |
| types | a loose categorization of place types based on keywords normally used in the LHOM index |
| matches | not used for non-aligned places (see aligned places) |
| start | generally the year 1200 AD, a token and largely meaningless date to vaguely indicate the 13th century, when Ibn Abī Uṣaybiʿa was writing, but the field is required for LP-TSV. Some places may be more ancient places mentioned in the text that no longer existed in the 13th century.  |
| title_source | LHOM = Emilie Savage-Smith, Simon Swain, and G. J. H. van Gelder, eds., _A Literary History of Medicine: The “Uyūn al-anbā” fī ṭabaqāt al-aṭibbā’ of Ibn Abī Uṣaybi’ah_, 5 vols. (Leiden: Brill, 2020). |
| title_uri | https://dh.brill.com/scholarlyeditions/library/urn:cts:arabicLit:0668IbnAbiUsaibia/, the open-access, CTS-enabled LHOM edition/translation|

## Warnings/Quirks
 - See particularly the note on the "start" field above.
 - Records are tentative and are still being reviewed. Feel free to create an issue here or in the source repo if you have corrections or suggestions.  



Also see [the general README](https://github.com/Hist-ME/URIs/blob/master/README.md) for this repo.