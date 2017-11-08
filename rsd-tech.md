# RSD Tech (Tom Klaver)

We could do a couple of things:
## Frontend
On Monday, SILO will come to discuss a new design for the RSD frontend, we could start thinking/planning/implementing the technology; keeping in mind
* Connection to current backend
* Search engine optimization
* Good analytics tools ([PiWik](https://piwik.org/)? Google analytics?)

## Backend
We have a backend for the RSD, consisting of a MongoDB for data storage, a Typescript/React administration frontend and Python/Flask as a layer in between. The plan is that on Thursday everybody is going to use this to fill some personal / project / software details so we need to test and streamline this flow. We may need to clean the data (schemas) a little bit. The data that has been added to Zotero the last few weeks has to be synchronized etc.

## Impact
We want to measure the impact of our software / projects. We can use a couple of data sources for this
* Publications in Zotero
* Github stats (stars/commits/activity/issues etc.)
* Libraries.io for depedency info from package managers (PyPi, npm, maven etc.)

We've already built the connectors/data acquisition in the Python backend but we need to figure out how to analyze/compare/present this data.

The RSD goals are still flexible so we can brainstorm a little about future plans. A few open questions:
* How to do integration with external parties (CIT/Groningen, KB Lab) (data sharing, analysis tools etc)
* Can we publish our data easily as linked data (JSON-LD?) 
* Can we aggregate usage statistics from our (web-based) tools in the RSD (with Piwik for example)
* ...
