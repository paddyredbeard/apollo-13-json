# Apollo 13 dot JSON

This project is a JSON representation of the **Apollo 13 Technical Air-to-Ground Transcript** originally published by NASA in April 1970.
Both a [minified version](apollo-13-tecatg.min.json) and a [pretty version](apollo-13-tecatg.json) of the JSON are provided.

## Source Material

This JSON version was adapted from the [plain text version](https://www.hq.nasa.gov/alsj/a13/AS13_TEC.txt) created by Heiko Kueffen.
PDF copies of this and other [Apollo 13 transcripts](https://www.hq.nasa.gov/alsj/a13/a13trans.html) are published on [NASA's Apollo 13 website](https://www.hq.nasa.gov/alsj/a13/a13.html).

## About the JSON Format

The JSON format presents Kueffen's plain text within a series of keyed objects:

- `metadata` - Metadata about this file and its sources.
- `preamble` - The title page and introduction text of the original transcript
- `acronyms` - The list of acronyms described in the original transcript
- `transcript` - An array containing each of the verbal communications between the air and ground crews

Each item in the `transcript` array, representing a single, one-way communication between the air and ground crews, is comprised of the following:

- `timestamp` - The hhh:mm:ss timestamp from Kueffen's text transcript representing mission hours, minutes, seconds
- `ddhhmmss` - A timestamp that restores the days, hours, minues, seconds format used in the original, typed transcript
- `speaker` - The acronym representing the person speaking
- `text` - The speaker's spoken words, transcribed

A technical description of this format is available in the [JSON schema](apollo-13-tecatg-schema.json) file.
The schema file was generated at <https://extendsclass.com/json-schema-validator.html> from the [sample JSON](_sample.json) file.

## Motivation

I created the JSON format in the hope it could be useful for creating a searchable index of verbal exchanges from the mission.

## Notable Exchanges Within the Transcript

### Stirring the Cryo Tanks and Initial Problem

Timestamp `055:52:58`: CAP COMM requests the air crew stir the oxygen tanks: "13, we've got one more item for you, when you get a chance. We'd like you to stir up your cryo tanks."

Timestamp `055:55:35`: Lovell reports the initial trouble with the Service Module's oxygen tank saying, "Houston, we've had a problem. We've had a MAIN B BUS UNDERVOLT."

### A Successfull Experiment

Timestamp `078:02:44`: Swigert, replying to the news that the S-IVB engine successfully crashed into the moon's surface, completing a planned, seismic experiment says, "Well, at least something worked on this flight."

### The Mailbox

Timestamp `080:22:13`: CAP COMM begins to describe the the procedure to modify the Command Module carbon dioxide scrubber to work in the Landing Module, "Yes. Me wish we could send you a kit and it would be kind of like putting a model airplane together or something. As it turns cut, this contraption will look like a mailbox when you get it all put together. [sic]"

### A Good Ship

Timestamp `142:30:50`: Mission control mentions contact was lost with Aquarious and Swigert remarks, "She sure was a good ship."

