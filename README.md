# Samply Maven

## How to use the internal MITRO maven repository

Maven uses several repositories:

1. $HOME/.m2/repository
2. the active repositories in your settings.xml and pom.xml
3. the central Maven Repository

If maven searches for artifacts this list of repository is searched in this
particular order. The first artifact that matches the requirements is used.

The parent POM can be used in another SAMPLY project by adding the parent artefact specification 
in the projects POM:

```xml
<parent>
    <groupId>de.samply</groupId>
    <artifactId>parent</artifactId>
    <version>${VERSION}</version>
</parent>
```

## License

Copyright 2020 The Samply Development Community

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.