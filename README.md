# MXCuBE code camp 2024-05-30: MXCuBE development workflows questionnaire

Questionnaire about development workflows for MXCuBE:
coding, testing, deployment, collaborating, etc.

It would be interesting if each facility could share how they handle those topics.
This is a suggestion for a questionnaire to gather this info.


### Questionnaire

* How to keep up to date with changes on GitHub upstream?
  * How often integrate (latest) changes from upstream?
  * Cherry picking specific changes (i.e.: important bug fixes)?

* How often do you contribute your improvements back to upstream GitHub?
  * Do you have your own forks of MXCuBE repositories?
    * If yes, do you use GitHub, GitLab or anything else like this?

* How to develop?

  * How far can you get working locally on your laptop only?
  * How often do you need to go test directly at the beamline?
  * How do you learn about the inner workings of MXCuBE? Is it enough to read the code?

* How to test?

  * Are you using simulated devices (Tango, Epics, etc.) to test the mxcube hardware objects?
    * What limitations or hurdles do you encounter when testing with mockup hardware compared to real hardware?
  * Do you have procedures for automatic tests?

* How much resources do you have?

  * How many MXCuBE developers are there in the facility?
    How many MX beamlines with MXCuBE do they have to take care of?

* How to deploy?

  * Python environments
    * Use conda environment? Or standard Python environment? venv, or Poetry?

  * Install Python dependencies?
    * With conda? pip? Poetry?

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
