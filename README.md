# MXCuBE code camp 2024-05-30: MXCuBE development workflows questionnaire

Questionnaire about development workflows for MXCuBE:
coding, testing, deployment, collaborating, etc.

It would be interesting if each facility could share how they handle those topics.
This way we can compare experiences, learn from each other,
identify common pain points, and collaborate better on MXCuBE.

All questions (besides the first two initial questions) are optional,
feel free to skip any question.

All questions expect free text answers,
feel free to expand on some questions if you feel it is necessary.

Each section has an "*additional comments*" question,
feel free to use it if the other questions do not correspond to what you want to write.


## General

1. ***Which facility?***

1. ***Which beamlines?***

1. ***What is the software stack?***

    Web or Qt (PyQt version, etc.),
    LIMS (ISPyB/EXI, ICAT, etc.),
    file formats (HDF5, CBF, etc.),
    real-time image viewer (Albula, Braggy, etc.),
    autoprocessing workflows,
    and so on


## Resources

How much developer resources do you have?

1. ***How many people work on MXCuBE?***

1. ***How many are software developers?***

1. ***How many beamlines with MXCuBE do they have to take care of?***

1. ***How many hours can they dedicate to working on MXCuBE?***

    In total. Per week, month, or year.

1. ***Do you have any additional comments?***


## Coding

How do you code for MXCuBE?

1. ***How far can you get coding locally using your computer or laptop only?***

1. ***How often do you need to go directly at the beamline to code (not test)?***

1. ***How do you learn about the inner workings of MXCuBE?***

    Is it enough to read the code?

1. ***Do you have any additional comments?***


## Collaboration

How do you collaborate on MXCuBE code?

1. ***How do you keep up to date with upstream changes on GitHub?***

1. ***How often do you integrate upstream changes?***

1. ***Do you only cherry pick specific changes?***

    For example important bug fixes only.

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


## Deployment

How do you deploy new MXCuBE code?

1. ***Do you use isolation environments for Python?***

    Do you use conda environment?
    Do you standard Python environment (venv, virtualenv, or Poetry)?
    Do you use Docker containers?

1. ***How do you install Python dependencies?***

    Do you install Python dependencies with conda, Poetry, pip?

1. ***How do you install JavaScript dependencies?***

1. ***What operating systems do you deploy on?***

    * Linux or something else? Which distribution? Which version?
    * Free choice or imposed by guidelines?
    * Centralised or local management (update cycle/package installation)?

1. ***Do you have infrastructure restrictions for deployment?***

    * Does you infrastructure/IT team restrict what you can use? Policies?
    * License restrictions?
    * Network restrictions?
    * Can you use Anaconda?
    * Do you have access to conda channels (package repositories), PyPI, npmjs.com?

1. ***Do you have access to specific infrastructure services?***

    * Do you have your own custom conda, PyPI, npm repositories?
    * Do you use Kubernetes, Ansible, or anything like that for deployment?

1. ***Do you have any additional comments?***


## Pain points

1. ***What are recurring pain points regarding MXCuBE development workflows?***

    In terms of coding, testing, deploying, collaborating, etc.

1. ***What do you think could be improved regarding MXCuBE development workflows?***

    In terms of coding, testing, deploying, collaborating, etc.

1. ***Do you have any additional comments?***


## Thanks!

Thank you for participating in this questionnaire.

Hopefully this will help us compare experiences, learn from each other,
identify common pain points, and improve collaboration on MXCuBE.
