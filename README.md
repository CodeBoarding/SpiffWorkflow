[![scorecard-score](https://github.com/recursionpharma/octo-guard-badges/blob/trunk/badges/repo/SpiffWorkflow/maturity_score.svg?raw=true)](https://infosec-docs.prod.rxrx.io/octoguard/scorecards/SpiffWorkflow)
[![scorecard-status](https://github.com/recursionpharma/octo-guard-badges/blob/trunk/badges/repo/SpiffWorkflow/scorecard_status.svg?raw=true)](https://infosec-docs.prod.rxrx.io/octoguard/scorecards/SpiffWorkflow)
## SpiffWorkflow
![Logo](./graphics/logo_med.png)

Spiff Workflow is a workflow engine implemented in pure Python. It is based on
the excellent work of the Workflow Patterns initiative. In 2020 and 2021,
extensive support was added for BPMN / DMN processing.

## Motivation
We created SpiffWorkflow to support the development of low-code business
applications in Python.  Using BPMN will allow non-developers to describe
complex workflow processes in a visual diagram, coupled with a powerful python
script engine that works seamlessly within the diagrams.  SpiffWorkflow can parse
these diagrams and execute them.  The ability for businesses to create
clear, coherent diagrams that drive an application has far reaching potential.
While multiple tools exist for doing this in Java, we believe that wide
adoption of the Python Language, and it's ease of use, create a winning
strategy for building Low-Code applications.


## Build status
[![SpiffWorkflow](https://github.com/sartography/SpiffWorkflow/actions/workflows/tests.yaml/badge.svg)](https://github.com/sartography/SpiffWorkflow/actions/workflows/tests.yaml)
[![Documentation Status](https://readthedocs.org/projects/spiffworkflow/badge/?version=latest)](http://spiffworkflow.readthedocs.io/en/latest/?badge=latest)
[![Issues](https://img.shields.io/github/issues/sartography/spiffworkflow)](https://github.com/sartography/SpiffWorkflow/issues)
[![Pull Requests](https://img.shields.io/github/issues-pr/sartography/spiffworkflow)](https://github.com/sartography/SpiffWorkflow/pulls)

## Code style

[![PEP8](https://img.shields.io/badge/code%20style-pep8-orange.svg)](https://www.python.org/dev/peps/pep-0008/)


## Dependencies
We've worked to minimize external dependencies.  We rely on lxml for parsing
XML Documents, and that's it!
<b>Built with</b>
- [lxml](https://lxml.de/)

## Features
* __BPMN__ - support for parsing BPMN diagrams, including the more complex
components, like pools and lanes, multi-instance tasks, sub-workflows, timer
events, signals, messages, boudary events and looping.
* __DMN__ - We have a baseline implementation of DMN that is well integrated
with our Python Execution Engine.
* __Python Workflows__ - We've retained support for building workflows directly
in code, or running workflows based on a internal json data structure.

_A complete list of the latest features is available with our [release notes](https://github.com/sartography/SpiffWorkflow/releases/tag/1.0) for
version 1.0._

## Code Examples and Documentation
Detailed documentation is available on [ReadTheDocs](https://spiffworkflow.readthedocs.io/en/latest/)
Also, checkout our [example application](https://github.com/sartography/spiff-example-cli), which we
reference extensively from the Documentation.

## Installation
```
pip install spiffworkflow
```

## Tests
```
pip install spiffworkflow[dev]
cd tests/SpiffWorkflow
coverage run --source=SpiffWorkflow -m unittest discover -v . "*Test.py"
```

## Support
You can find us on Discord at https://discord.gg/BYHcc7PpUC

Commercial support for SpiffWorkflow is available from
[Sartography](https://sartography.com)

## Contribute
Pull Requests are and always will be welcome!

Please check your formatting, assure that all tests are passing, and include
any additional tests that can demonstrate the new code you created is working
as expected.  If applicable, please reference the issue number in your pull
request.

## Credits and Thanks

Samuel Abels (@knipknap) for creating SpiffWorkflow and maintaining it for over
a decade.

Matthew Hampton (@matthewhampton) for his initial contributions around BPMN
parsing and execution.

The University of Virginia for allowing us to take on the mammoth task of
building a general-purpose workflow system for BPMN, and allowing us to
contribute that back to the open source community. In particular, we would like
to thank [Ron Hutchins](https://www.linkedin.com/in/ron-hutchins-b19603123/),
for his trust and support.  Without him our efforts would not be possible.

Bruce Silver, the author of BPMN Quick and Easy Using Method and Style, whose
work we referenced extensively as we made implementation decisions and
educated ourselves on the BPMN and DMN standards.

The BPMN.js library, without which we would not have the tools to effectively
build out our models, embed an editor in our application, and pull this mad
mess together.

Kelly McDonald (@w4kpm) who dove deeper into the core of SpiffWorkflow than
anyone else, and was instrumental in helping us get some of these major
enhancements working correctly.

Thanks also to the many contributions from our community.  Large and small.
From Ziad (@ziadsawalha) in the early days to Elizabeth (@essweine) more
recently.  It is good to be a part of this long lived and strong
community.


## License
GNU LESSER GENERAL PUBLIC LICENSE
