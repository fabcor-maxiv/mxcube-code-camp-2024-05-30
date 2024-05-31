# MXCuBE code camp 2024-05-30

## MXCuBE workflows

About workflows for MXCuBE: development, deployment, testing, collaboration, etc.


### Discussion

Participants:

* Alessandro (Elettra)
* Dan (Soleil)
* Fabien (MAX IV)
* Laís (ESS)

Notes:

_To be completed..._


### Questionnaire

It would be interesting if each facility could share how they handle those topics.

This is a suggestion for a questionnaire to gather this info.

* How to keep up to date with changes on GitHub upstream?
  * How often integrate (latest) changes from upstream?
  * Cherry picking specific changes (i.e.: important bug fixes)?

* How often do you contribute your improvements back to upstream GitHub?

* How to develop?

  * How far can you get working locally on your laptop only?
  * How often do you need to go test directly at the beamline?

* How to deploy?

  * Python environments
    * Use conda environment? Or standard Python environment? venv, or Poetry?

  * Install Python dependencies?
    * With conda? pip? Poetry?

  * Same question for Javascript dependencies?

  * Infrastructure restrictions?
    * Does you infrastructure/IT team restrict what you can use? Policies?
    * License restrictions
    * Network restrictions
    * Can you use Anaconda?
    * Do you have access to conda channels (package repositories)? PyPI? npmjs.com?

  * Infrastructure services
    * Do you have your own custom conda, PyPI, npm repositories?

  * Kubernetes, Ansible
