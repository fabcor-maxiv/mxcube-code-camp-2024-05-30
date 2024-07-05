# MXCuBE code camp 2024-05-30: MXCuBE development workflows questionnaire

Questionnaire about development workflows for MXCuBE:
coding, testing, deployment, collaborating, etc.

It would be interesting if each facility could share how they handle those topics.
This is a suggestion for a questionnaire to gather this info.


## General

1. ***Which facility (and beamlines)?***

    Specific both name of the facility and beamline(s)
    if you intend to fill in the form multiple times (one per beamline or beamline group).

2. ***How many beamlines?***


## Resources

How much resources do you have?

1. ***How many people working on MXCuBE?***

1. ***How many are software developers?***

1. ***How many MX beamlines with MXCuBE do they have to take care of?***

1. ***How many hours can they dedicate to work on MXCuBE development?***

    Per week, month, or year.


## Coding

How to code?

1. ***How far can you get working locally on your laptop only?***

1. ***How often do you need to go test directly at the beamline?***

1. ***How do you learn about the inner workings of MXCuBE?***

    Is it enough to read the code?


## Collaboration

How to collaborate?

1. ***How do you keep up to date with changes on GitHub upstream?***

1. ***How often integrate (latest) changes from upstream?***

1. ***Do you only cherry pick specific changes?***

    i.e.: important bug fixes

1. ***Do you have your own forks of MXCuBE repositories?***

    If yes, do you use GitHub, GitLab or anything else like this?

1. ***How often do you contribute your improvements back to upstream GitHub?***


## Test

How to test?

1. ***How do you test new code?***

1. ***Are you using simulated devices (Tango, Epics, etc.) to test the mxcube hardware objects?***

1. ***What limitations or hurdles do you encounter when testing with mockup hardware?***

    Compared to real hardware.

1. ***Do you have procedures for automatic tests?***

    For example in a CI/CD toolchain.


### Deployment

How to deploy?

1. ***Python environments***

    Use conda environment? Or standard Python environment? venv, or Poetry?

1. ***Install Python dependencies?***

    With conda? pip? Poetry?

1. ***Install Javascript dependencies?***

1. ***Choice of OS***

    * Linux or something else? Which distribution?
    * Free choice or imposed by guidelines?
    * Centralised or local managment (update cycle/package installation)?

1. ***Infrastructure restrictions?***

    * Does you infrastructure/IT team restrict what you can use? Policies?
    * License restrictions
    * Network restrictions
    * Can you use Anaconda?
    * Do you have access to conda channels (package repositories)? PyPI? npmjs.com?

1. ***Infrastructure services***

    * Do you have your own custom conda, PyPI, npm repositories?
    * Do you use Kubernetes, Ansible, or anything like that for deployment?
