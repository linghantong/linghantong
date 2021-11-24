This project is the main hub to all kinds of documentation related to the Jackson JSON Processor.

Tutorials
For your first steps in understanding how to use Jackson, following tutorials are good places to start:

Baeldung Jackson JSON Tutorial
Jackson in N minutes (README for jackson-databind project)
Jenkov.com Jackson Tutorial
JournalDev JacksonTutorial
LogicBig.com Jackson Tutorial
Mkyong.com's Jackson Tutorial (part of larger Java JSON Tutorials
StudyTrails Jackson Introduction
General
Annotations
Jackson Annotations (links to core/databind/JAXB annotations)
Customize your Java-JSON serialization using Jackson Annotations
Advanced Jackson annotations
Frameworks, Platforms
Jackson on Android (proguard definitions)
JVM Languages beyond Java
(need links to Scala, Kotlin, Clojure tutorials, articles)

Other
Where are the Javadocs?
Presentations by Jackson Team, friends
Documentation under Jackson GH projects
Jackson project hub has links to all active Jackson projects. These projects contain plenty of project-specific documentation, such as:

Core Annotations
List of Jackson Core Annotations
Streaming API
On/off features: JsonFactory.Features, JsonGenerator.Features,JsonParser.Features.
Databind
Databind Annotations
On/off features: DeserializationFeatures, SerializationFeatures, MapperFeatures.
External (off-GitHub) documentation
Blogs that regularly write about Jackson include:

Cowtowncoder @Medium
CowTalk Blog (old, getting obsolete)
And here are good articles around the web:

General usage
Jackson JSON Tutorial by Eugen Paraschiv
Jackson - Installation at Jenkov.com
Processing JSON with Jackson (DZone)
Jackson jr for casual JSON processing
Jackson annotations:
A Guide to Jackson Annotations by Baeldung
Jackson Annotations at Jenkov.com
Streaming reading/writing
Customize serialization with Jackson Annotations
Streaming API
Jackson - JsonParser
Jackson - JsonGenerator
Polymorphic type handling:
Custom polymorphic type handling with Jackson (2013 Sep)
Data formats beyond JSON
Writing CSV using Jackson CSVMapper & Mixin annotations
Reading, Writing Java Properties with Jackson
Read YAML in Java with Jackson
Platform-specific Jackson integration
Apache CXF
Configuring Snake Case naming
Participating
The easiest ways to participate is to join one of Jackson mailing lists (Jackson google groups):

Jackson Announce: Announcement-only list for new Jackson releases, meetups and other events related to Jackson
Jackson User: List dedicated for discussion on Jackson usage
Jackson Dev: List for developers of Jackson core components and modules, discussing implementation details, API changes.
There are other related lists and forums as well:

Smile Format Discussion: List for discussing details of the binary JSON format called Smile (see Smile Specificat
ion)
Jackson Users is a Jackson-specific discussion forum for usage questions.
Sample code
See (External) Jackson Sample Code.

On Jackson versioning
Note that there are two major Jackson versions: 1.x (1.0 - 1.9) and 2.x (2.0 - 2.9). These versions can co-exist as they are located in different Java packages and use different jar naming and Maven group/artifact ids. But this means that you have to make sure that all components in use have matching major versions: specifically, Jackson 2.x code does NOT understand or support Jackson 1.x annotations, or vice versa.

Minor versions (like 2.1 and 2.2) are backwards compatible with respect to public API: old code should work without recompilation, if (but only if) it relies on external API; public methods, annotations. When overriding internal functionality, we try hard to maintain backwards compatibility between adjacent minor versions; need for changes is indicated by deprecating internal methods. Recompilation is thus recommended when extending by sub-classing, for example.

Misc other
Old Jackson home is still occasionally linked to from various places -- please DO NOT link from new documentation.
Jackson Git Hub is the... The Hub for all stuff, including this project.