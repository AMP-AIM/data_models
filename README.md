# Data Models

This repository contains 3 major files:

1. `ampaim.model.csv`: The CSV representation of the AMP AIM data model. This file 
is created by the collective effort of data curators and annotators from the AMP AIM 
and is used to create the JSON-LD representation of the data model.


2. `ampaim.model.jsonld`: The JSON-LD representation of the data model, which is 
automatically created from the CSV data model using the schematic CLI. More details 
on how to convert the CSV data model to the JSON-LD data model can be 
found [here](https://sage-schematic.readthedocs.io/en/develop/cli_reference.html#schematic-schema-convert). 
This is the central schema (data model) which will be used to power the 
generation of metadata manifest templates for various data types (e.g., `scRNA-seq Level 1`) 
from the schema.


3. `config.yml`: A template version of the schematic-compatible configuration file, 
which allows users to specify values for application-specific keys (e.g., path 
to Synapse configuration file) and project-specific keys (e.g., Synapse 
fileview for community project). A description of what the various keys in this 
file represent can be found in the [Fill in Configuration File(s)](https://sage-schematic.readthedocs.io/en/develop/README.html#fill-in-configuration-file-s) 
section of the schematic [docs](https://sage-schematic.readthedocs.io/en/develop/index.html).