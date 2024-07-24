# VersioningSchema

A schema for defining the semantics of a version string.

----

Version strings have many semantics that are not obvious from the string itself.
Therefore, external metadata is needed to be able to utilise any version string.

For instance, it is not immediately obvious that, in SemVer, version '1.0.1-v2' is ordered before version '1.0.1'.

This is what a **VersioningSchema** is for.

Here are some aspects of a version string that this schema is used to define:

- The type of each segment of a version string
- Which segments of a version string are required
- How version strings are ordered or compared

----

The main schema definition file is found at [`schema.json`](schema.json).
This file defines the expected format of a definition for a semantic version string.

Sample schema files can be found in the [`examples`](examples/) directory.
For instance, [`examples/semver.schema.json`](examples/semver.schema.json) defines the expected format of a [SemVer](https://semver.org) version string.
