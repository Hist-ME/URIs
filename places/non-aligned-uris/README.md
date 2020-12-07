# Unaligned place URIs

See also [the general README](https://github.com/Hist-ME/URIs/blob/master/README.md) for this repo.

This is a place to publish place URIs from different projects. The idea is to make URIs and descriptions of places 
used in projects publicly available so that other projects can start to align or link their own place entities
to these.

## Simple TSV format

Your data should have at least two columns: `uri` and `description`:

### uri

The URL of the place in your project
 
### description

The name or short description of the place that enables other users to quickly understand
which place you are referring to.

Your data can have more columns with additional information.

## LP-TSV format

Data in [LP-TSV format](https://github.com/LinkedPasts/linked-places/blob/master/tsv_0.2.md) can be uploaded to
the [World Historical Gazetteer](http://whgazetteer.org/tutorials/) where you can use the reconciliation tool
to align your place data with existing gazetteers like Getty TGN, Wikidata and others and then download the augmented
data with added references.

LP-TSV data should have at least four columns: `id`, `title`, `title_source` and `start`:

### id

Your internal project identifier (can also be a URL)

### title

A single "preferred" place name or desciption

### title_source

A label or short citation for source of the title toponym (could be your project name)

### start

Earliest relevant date in ISO 8601 form (YYYY-MM-DD); omit day and/or month as required. 
Note: this date relates to the attestation of the place in your project data. It is not the date the place was created.

Your data can not have columns that are not part of the LP-TSV format.

Note: Some of the "encouraged" and "optional" columns allowed by the LP-TSV format are not currently supported by the World Historical Gazetteer TSV-parser.
