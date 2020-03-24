# Settings Manager
Manage application settings and preferences with a JSON settings file.

# JSON parsing
RapidJSON library is used. File parsing uses parse flags:

| Parse Flag | Description |
|:--|:--|
|rapidjson::kParseCommentsFlag|Allow one-line (//) and multi-line (/**‍/) comments.|
|rapidjson::kParseTrailingCommasFlag|Allow trailing commas at the end of objects and arrays.|
See https://rapidjson.org/namespacerapidjson.html#a81379eb4e94a0386d71d15fda882ebc9

# Settings Storage Data Structure
`rapidjson::Document` is used to store settings. 

# Why is RapidJSON used?
The hjson library was also considered as an option because it allows more flexible json settings file. rapidJSON is often used as a high performance JSON parsing. Even though each JSON library serves different uses, using two different JSON libraries seemed redundant and confusing. 