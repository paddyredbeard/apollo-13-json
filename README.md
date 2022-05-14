# Apollo 13 dot JSON

This project is a JSON representation of the **Apollo 13 Technical Air-to-Ground Transcript** originally published by NASA in April 1970.

## Source Material

This JSON version was adapted from the [plain text version](https://www.hq.nasa.gov/alsj/a13/AS13_TEC.txt) created by Heiko Kueffen.
PDF copies of this and other [Apollo 13 transcripts](https://www.hq.nasa.gov/alsj/a13/a13trans.html) are published on [NASA's Apollo 13 website](https://www.hq.nasa.gov/alsj/a13/a13.html).

## About the JSON Format

The JSON format presents Kueffen's plain text within a series of keyed objects:

- `metadata` - Metadata about this file and it's sources.
- `preamble` - The title page and introduction text of the original transcript
- `acronyms` - The list of acronyms described in the original transcript
- `transcript` - An array listing each of the verbal communications between the air and ground crews

A technical description of this format is available in the [JSON schema](apollo-13-tecatg-schema.json) file.
The schema file was generated at <https://extendsclass.com/json-schema-validator.html> from the [_sample.json](_sample.json) file.

## Motivation

I created the JSON format in the hope it could be useful for creating a searchable index of verbal exchanges from the mission.

## Notable Exchanges Within the Transcript

The initial trouble with the Service Module's oxygen tank begins at timestamp `055:55:20`.
