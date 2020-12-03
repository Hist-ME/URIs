# URIs
This is a place to align URIs among different projects for persons, places, works, manuscripts, and potentially other entities related to the historical Middle East.

## How to use these URIs
Here you'll find folders for each entity containing **simple TSV tables with at least three columns**. Each row represents a relationship between the URIs in each of the columns. The columns are not ordered: which URI appears in which column does not matter. Each URI may appear multiple times in the spreadsheet when it has relationships to additional URIs. 

You can import this into the spreadsheet editor or data format of your choice and use lookup, filter, or similar functions to search for one URI and get related URIs from other domains (projects). Note: When searching for URIs, make sure to take into account both http:// and https:// versions as well as with or without www . In regex, this can be done with `https?://(www\.)?`.

**This alignment assumes** only that the URIs are *related* (formally, [dc:relation](http://purl.org/dc/elements/1.1/relation) can be asserted). It does *not* always mean that the URIs refer to exactly the same entity. For example, different projects might use different strategies to identify pseudonymous authors of works (e.g., "Pseudo-Chrysostom" vs. "Author of Homily X") or to connect historical places with geographical locations. These differing strategies mean that related URIs might refer to somewhat differently conceived entities. Formally speaking, [owl:sameAs](https://www.w3.org/TR/owl-ref/#sameAs-def) cannot be asserted. This is also the case because the list may contain URIs that are used to identify and disambiguate entities (such as a Wikipedia page about a place or a biographical notice in [*Onomasticon Arabicum*](https://onomasticon.irht.cnrs.fr/)) but are not actually URIs identifying the same kind of entity (a bibliographic resource URI vs. a place or person URI). See the [description field](#description) below.

Exports into other formats (such as RDF) might be provided in this repository, but **for now, the canonical data is in the TSV spreadsheets** and other formats are derivative.

### Example
| uri* | related-uri* | according-to* | description
| --- | --- | --- | --- |
| https://usaybia.net/person/32 | http://viaf.org/viaf/81975562 | https://usaybia.net | is probably the same as |
| https://usaybia.net/person/32 | https://dx.doi.org/10.1163/1573-3912_ei3_COM_24150 | https://usaybia.net | is the primary entity described by |

**\*** indicates required fields.

#### uri*
*required:* The URI of the entity (person, place, etc.) in your system that is being related to another URI.

#### related-uri*
*required:* The URI of the related entity in another system.

#### according-to*
*required:* A URI identifying the project, team, or person responsible for asserting the relationship between the URIs in the first two columns.

#### description
*optional:* An informal description of the relationship between the two URIs, for example, "is probably the same as" or "is the primary entity described by". This provides guidance to other projects who may be trying to align their URIs with the ones mentioned. It may also be the basis for creating RDF triples in the future. Please try to keep your descriptions consistent for rows describing the same relationship.

## How to contribute URIs
 1. Create a **new branch** (if you're a member) or **fork** this repo. To become a member, please contact one of the organization owners.
 2. **Add a new TSV file** to the relevant folder, named [yourprojectnameorwebsite].tsv, with the columns mentioned above. 
 3. **Create a pull request** to merge your updated spreadsheet into the master branch.

### Guidelines
 1. If a URI has multiple related URIs, add a separate row for each relationship.
 2. Please don't include URIs that don't have any related URIs (blank cells). They aren't useful here unless they're matched.
 3. At least one URI in each row (yours or the related one) should resolve to a URL with sufficient information to identify the entity. 
 4. Don't add names or other non-URI identifiers to the spreadsheet. This is to make sure all identifications are done on the basis of the URIs themselves, not extra information in the spreadsheet.

## Questions? 
Please file a new [issue](https://github.com/Hist-ME/URIs/issues).
If you believe a relationship in the spreadsheet is incorrect, please file an issue mentioning the relevant URIs and the line number in the spreadsheet.

## Discussion
Discussion for members of the Hist-ME Github organization is conducted on the team discussion page. If you're not a member and would like to be, please file an [issue](https://github.com/Hist-ME/URIs/issues).
