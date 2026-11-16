ECDICT lookup data

The JSON files are compact shards derived from ECDICT. The app loads only the
shard matching the first two English letters and keeps it in memory for later
lookups. Entries contain short Chinese meanings by part of speech. The
converter ignores bracket-labeled specialist entries and never truncates a
longer meaning.

To regenerate the files, download ecdict.csv from:
https://github.com/skywind3000/ECDICT

Then run from the project directory:
.\scripts\build-ecdict.ps1 -SourceCsv .\ecdict.csv

See ECDICT-LICENSE.txt for source attribution and the MIT license.
