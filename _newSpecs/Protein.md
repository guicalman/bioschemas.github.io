---
description: "This protein specification presents the usage of the generic type BiologicalEntity\
  \ by the biological type \u201Cprotein\u201D. Please be aware \u201Cprotein\u201D\
  \ is NOT a schema.org type but a BiologicalEntity profile."
edit_url: https://github.com/BioSchemas/bioschemas.github.io/edit/master/_newSpecs/Protein.md
extended_props:
  CreativeWork:
  - bsc_dec: ''
    cardinality: MANY
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - CreativeWork
    - URL
    marginality: Recommended
    name: citation
    sdo_desc: A citation or reference to another creative work, such as another publication,
      web page, scholarly article, etc.
  - bsc_dec: ''
    cardinality: ONE
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - Date
    - DateTime
    marginality: Optional
    name: dateCreated
    sdo_desc: The date on which the CreativeWork was created or the item was added
      to a DataFeed.
  - bsc_dec: ''
    cardinality: ONE
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - Date
    - DateTime
    marginality: Optional
    name: dateModified
    sdo_desc: The date on which the CreativeWork was most recently modified or when
      the item's entry was modified within a DataFeed.
  - bsc_dec: ''
    cardinality: MANY
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - BiologicalEntity
    marginality: Optional
    name: hasPart
    sdo_desc: Indicates a CreativeWork that is (in some sense) a part of this CreativeWork.
  - bsc_dec: ''
    cardinality: MANY
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - BiologicalEntity
    marginality: Optional
    name: isPartOf
    sdo_desc: Indicates a CreativeWork that this CreativeWork is (in some sense) part
      of.
  Thing:
  - bsc_dec: ''
    cardinality: MANY
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - Text
    marginality: Recommended
    name: alternateName
    sdo_desc: An alias for the item.
  - bsc_dec: ''
    cardinality: ONE
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - Text
    marginality: Recommended
    name: description
    sdo_desc: A description of the item.
  - bsc_dec: ''
    cardinality: ONE
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - PropertyValue
    - Text
    - URL
    marginality: Minimum
    name: identifier
    sdo_desc: The identifier property represents any kind of identifier for any kind
      of <a class="localLink" href="http://schema.org/Thing">Thing</a>, such as ISBNs,
      GTIN codes, UUIDs etc. Schema.org provides dedicated properties for representing
      many of these, either as textual strings or as URL (URI) links. See <a href="/docs/datamodel.html#identifierBg">background
      notes</a> for more details.
  - bsc_dec: ''
    cardinality: MANY
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - ImageObject
    - URL
    marginality: Recommended
    name: image
    sdo_desc: An image of the item. This can be a <a class="localLink" href="http://schema.org/URL">URL</a>
      or a fully described <a class="localLink" href="http://schema.org/ImageObject">ImageObject</a>.
  - bsc_dec: ''
    cardinality: ONE
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - Text
    marginality: Recommended
    name: name
    sdo_desc: The name of the item.
  - bsc_dec: ''
    cardinality: MANY
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - URL
    marginality: Recommended
    name: sameAs
    sdo_desc: URL of a reference Web page that unambiguously indicates the item's
      identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official
      website.
  - bsc_dec: ''
    cardinality: ONE
    controlled_vocab:
      ontologies: []
      terms: []
    expected_type:
    - URL
    marginality: Recommended
    name: url
    sdo_desc: URL of the item.
g_mapping_file: Protein Mapping
gh_folder: https://github.com/BioSchemas/Protein
gh_tasks: https://github.com/BioSchemas/bioschemas/labels/type%3A%20Protein
hierarchy:
- CreativeWork
- Thing
layout: new_spec_detail
name: Protein
new_props:
- bsc_dec: ''
  cardinality: MANY
  controlled_vocab:
    ontologies: []
    terms: []
  expected_type:
  - DataDownload
  marginality: Optional
  name: distribution
  sdo_desc: A downloadable form of this entity, at a specific location, in a specific
    format
- bsc_dec: ''
  cardinality: MANY
  controlled_vocab:
    ontologies: []
    terms: []
  expected_type:
  - MedicalCondition
  - URL
  marginality: Optional
  name: associatedDisease
  sdo_desc: Disease associated to this protein feature
- bsc_dec: ''
  cardinality: ONE
  controlled_vocab:
    ontologies: []
    terms: []
  expected_type:
  - QuantitativeValue
  marginality: Recommended
  name: biocoordinates
  sdo_desc: 'Coordinates in a 1 or 2D space, for instance length/coordinates in a
    sequence.  Usage (example): Use a QuantitativeValue with properties minValue and
    maxValue for a region or value for a site in a Protein. Use it only with value
    for a protein length.'
- bsc_dec: ''
  cardinality: MANY
  controlled_vocab:
    ontologies: []
    terms: []
  expected_type:
  - Text
  marginality: Minimum
  name: biologicalType
  sdo_desc: List with types preferably supported by BioSchemas-> enumeration list
    of values maintained on a wikipage (cf accessibilityAPI in schema.org for implementation).
    If the value is not on the list then the data will still be parsed but only generic
    properties will be validated. {population,individual,tissue,cell,molecule,protein,nucleic
    acid}
- bsc_dec: ''
  cardinality: MANY
  controlled_vocab:
    ontologies: []
    terms: []
  expected_type:
  - Thing
  marginality: Optional
  name: crossReference
  sdo_desc: 'A pointer to another, somehow related entity. Usage: Whenever isBasedOn/isBasisFor,
    isPartOf/hasPart, citation or any other more specific does not work.'
- bsc_dec: ''
  cardinality: MANY
  controlled_vocab:
    ontologies: []
    terms: []
  expected_type:
  - Text
  - URL
  - PropertyValue
  marginality: Optional
  name: representation
  sdo_desc: Representation of this entity. For instance, chemical structure or sequence
- bsc_dec: ''
  cardinality: MANY
  controlled_vocab:
    ontologies: []
    terms:
    - 'Yes'
  expected_type:
  - URL
  marginality: Optional
  name: taxon
  sdo_desc: A url pointing to NCBI Taxonomy or a taxonomic resource
- bsc_dec: ''
  cardinality: ONE
  controlled_vocab:
    ontologies: []
    terms: []
  expected_type:
  - Thing
  marginality: Recommended
  name: isMentionedIn
  sdo_desc: CreativeWork, Dataset, collection mentioning this entity  Inverse of:mentions
- bsc_dec: ''
  cardinality: MANY
  controlled_vocab:
    ontologies: []
    terms: []
  expected_type:
  - PropertyValue
  marginality: Optional
  name: additionalProperty
  sdo_desc: A property-value pair representing an additional characteristics of the
    entitity, e.g. a product feature or another characteristic for which there is
    no matching property in schema.org.  Avoid it if possible, otherwise use it carefully.
    Please keep in mind that Bioschemas does not pretend to model every single possible
    field but mainly those useful for discoverability, summarization and accessibility.
parent_type: CreativeWork
spec_mapping_url: https://docs.google.com/spreadsheets/d/1QQH4AkzdwPT1Qt5OLmH5HosLpkFU7khwE4Ql9_Cb9ZQ/edit?usp=drivesdk
spec_type: Profile
status: revision
subtitle: "Bioschemas specification describing the usage of BiologicalEntity for the\
  \ \u201CProtein\u201D biological type. "
version: 0.0.1
---