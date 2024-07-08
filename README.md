# MXCuBE code camp 2024-05-30: MXCuBE development workflows questionnaire

Questionnaire about development workflows for MXCuBE:
coding, testing, deployment, collaborating, etc.

It would be interesting if each facility could share how they handle those topics.
This way we can compare experiences, learn from each other,
identify common pain points, and collaborate better on MXCuBE.

Feel free to fill in the questionnaire multiple times,
if you want to give different answers for each beamline (or group of beamlines).

All questions (besides the first two inital questions) are optional,
feel free to skip any question.

All questions expect free text answers,
feel free to expand on some questions if you feel it is necessary.


## General

1. ***Which facility (and beamlines)?***

2. ***Which beamlines?***

    Feel free to fill in the questionnaire multiple times,
    if you want to give different answers for each beamline (or group of beamlines).


## Resources

How much developer resources do you have?

1. ***How many people work on MXCuBE?***

1. ***How many are software developers?***

1. ***How many beamlines with MXCuBE do they have to take care of?***

1. ***How many hours can they dedicate to working on MXCuBE?***

    Per week, month, or year.

1. ***Do you have any additional comments?***


## Coding

How do you code for MXCuBE?

1. ***How far can you get coding locally on your laptop only?***

1. ***How often do you need to go directly at the beamline to code (not test)?***

1. ***How do you learn about the inner workings of MXCuBE?***

    Is it enough to read the code?

1. ***Do you have any additional comments?***


## Collaboration

How do you collaborate on MXCuBE code?

1. ***How do you keep up to date with upstream changes on GitHub?***

1. ***How often do you integrate upstream changes?***

1. ***Do you only cherry pick specific changes?***

    i.e.: important bug fixes

1. ***Do you have your own forks of MXCuBE repositories?***

    If yes, do you use GitHub, GitLab or anything else like this?
    Are these forks publicly accessible?

1. ***How often do you contribute your improvements back to upstream GitHub?***

1. ***How confident do you feel using the collaboration tools?***

    For example: git and GitHub, pre-commit hooks, linting tools, formatters, and so on.

1. ***Do you have any additional comments?***


## Test

How do you test new MXCuBE code?

1. ***How do you test new code?***

1. ***Do you use simulated devices (Tango, Epics, etc.) to test hardware objects?***

1. ***What limitations or hurdles do you encounter when testing with mockup hardware?***

    Compared to real hardware.

1. ***Do you have procedures for automated tests?***

    For example in a CI/CD toolchain.

1. ***Do you have any additional comments?***


### Deployment

How do you deploy new MXCuBE code?

1. ***Do you use isolation environments for Python?***

    Do you use conda environment?
    Do you standard Python environment (venv, virtualenv, or Poetry)?
    Do you use Docker containers?

1. ***How do you install Python dependencies?***

    Do you install Python dependencies with conda, Poetry, pip?

1. ***How do you install Javascript dependencies?***

1. ***What operating systems do you deploy on?***

    * Linux or something else? Which distribution?
    * Free choice or imposed by guidelines?
    * Centralised or local managment (update cycle/package installation)?

1. ***Do you have infrastructure restrictions for deployment?***

    * Does you infrastructure/IT team restrict what you can use? Policies?
    * License restrictions?
    * Network restrictions?
    * Can you use Anaconda?
    * Do you have access to conda channels (package repositories), PyPI, npmjs.com?

1. ***Infrastructure services***

    * Do you have your own custom conda, PyPI, npm repositories?
    * Do you use Kubernetes, Ansible, or anything like that for deployment?

1. ***Do you have any additional comments?***


## General pain points

1. ***What are recurring pain points regarding MXCuBE development workflows?***

    In terms of coding, testing, deploying, collaborating, etc.
    What could be improved?

1. ***Do you have any additional comments?***


## Thanks!

Thank you for participating in this questionnaire.

Hopefully this will help us compare experiences, learn from each other,
identify common pain points, and improve collaboration on MXCuBE.
