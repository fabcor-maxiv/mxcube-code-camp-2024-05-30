# MXCuBE code camp 2024-05-30

## MXCuBE workflows

About workflows for MXCuBE: development, deployment, testing, collaboration, etc.


### Discussion

#### Participants

* Alessandro (Elettra)
* Andrey (Desy)
* Dan (Soleil)
* Fabien (MAX IV)
* Laís (ESS)

#### Notes

_To be completed..._

* Dan:

  What is a good development workflow?

* Fabien:

  At BioMAX, no users on Monday, Tuesday and sometimes Wednesday
  so it is possible to use the beamline to develop software.
  This time is shared with beamline staff and other commissioning work.
  Rest of the week to clean up code and make pull requests
  or work on other tasks.

  At MicroMAX, most coding work is done with emulators assembled in Docker Compose.
  Final tests are done at the beamline.

* Alessandro:

  How to keep up to date with changes upstream on GitHub?

* Fabien:

  ESRF talked a bit about their workflow in their talk the day before.
  They typically rebase their own changes on top of upstream every two weeks.

  At MAX IV, we have a similar workflow, we rebase every two weeks.
  This is okay for now, but we will see if it is sustainable over time.

* Alessandro:

  Is it possible to make a pull request on GitHub from the code on internal GitLab?

* Fabien:

  As far as I know, it is not possible.

  It is important to get very comfortable with git,
  to handle these kinds of cases, switching between multiple repositories.

* Laís:

  It is worth investing time to learn git,
  it makes work much easier, especially in a collaboration like MXCuBE.

* Dan, presents UML diagram of some of the most important classes in MXCuBE-Core:

  Diagrams are usefull tools when trying to understand how the various components of the MXCuBE app interact. I tried using Pyrevese to automaitly generate class diagrams. This methods is fast and although it can provide some usefull information, the resulting diagrams were incomplete, with many relationships between classes missing.
  I also tried making class diagrams "by hand", using Gaphor but doing this for all classes in MXCuBE takes time so I only did this for the sample changer.  
  One ideea for visualising class diagram would be to write a script that would extract this information from the code and store it in Neo4J database. I chose Neo4J because I know it quite well having worked with it in the past and it's a natural fit for data structures such as class diagrams. This would allow the visualisation off any set of classes and their relationships. This approach would be much faster than drawing the whole MXCuBE app class diagram in Gaphor but I'm not sure if the overall utility for the project is worth the time. At this point it's just an idea that could make querying info about the classes, the components and their interactions easyer and faster than digging through the code. I could put some more effort into it, if there is interest.

* Laís:
  I would be interested in such diagram.

* Fabien:

  In principle it should be feasible with Sphinx documentation system.
  I have tried it, but the resulting diagram was not readable.
  I should maybe try it again.

_To be completed..._


### Questionnaire

It would be interesting if each facility could share how they handle those topics.

This is a suggestion for a questionnaire to gather this info.

* How to keep up to date with changes on GitHub upstream?
  * How often integrate (latest) changes from upstream?
  * Cherry picking specific changes (i.e.: important bug fixes)?

* How often do you contribute your improvements back to upstream GitHub?
  * Do you have your own forks of MXCuBE repositories?
    * If yes, do you use GitHub, GitLab or anything else like this?

* How to develop?

  * How far can you get working locally on your laptop only?
  * How often do you need to go test directly at the beamline?
  * What role does reverse engineering play in the developmet process? As a new developer to the MXCuBE project I often find miself tring to figure out how the various components work and how they interface with eachother. Most of this information is not yet documented. Are there any best practices for how to speed up learning about the inner workings of the MXCuBE App?
  * Should we write a user manual and a developer manual or should we keep all documantation in a single place (mxcubewed/docs)  

* How to test?

  * Are you using simulated devices (Tango, Epics, etc.) to test the mxcube hardware objects? Waht are the limitations othe mockup hardware objects when testing ?
  * Do you have procedures for automatic tests?

* How much resources do you have?

  * How many MXCuBE developers are there in the facility?
    How many MX beamlines with MXCuBE do they have to take care of?

* How to deploy?

  * Python environments
    * Use conda environment? Or standard Python environment? venv, or Poetry?

  * Install Python dependencies?
    * With conda? pip? Poetry?
    * How often should we do a poetry install? (as an example if I see that the poetry.lock file changed after I do a git pull, then I also do a poetry install but I'm not yet sure how good is this practice)

  * Same question for Javascript dependencies?

  * Choose of OS
    * Linux/something else? Which distribution?
    * Free choice or imposed by guidlines?
    * Centrralised or local managment (update cycle/package installation)?     

  * Infrastructure restrictions?
    * Does you infrastructure/IT team restrict what you can use? Policies?
    * License restrictions
    * Network restrictions
    * Can you use Anaconda?
    * Do you have access to conda channels (package repositories)? PyPI? npmjs.com?

  * Infrastructure services
    * Do you have your own custom conda, PyPI, npm repositories?

  * Do you use Kubernetes, Ansible, or anything like that for deployment?
