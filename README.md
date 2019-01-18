# Digital DNA Toolbox

<!--
[![Travis Status](https://travis-ci.org/scikit-learn-contrib/project-template.svg?branch=master)](https://travis-ci.org/scikit-learn-contrib/project-template)
[![Coveralls Status](https://coveralls.io/repos/scikit-learn-contrib/project-template/badge.svg?branch=master&service=github)](https://coveralls.io/r/scikit-learn-contrib/project-template)
[![CircleCI Status](https://circleci.com/gh/scikit-learn-contrib/project-template.svg?style=shield&circle-token=:circle-token)](https://circleci.com/gh/scikit-learn-contrib/project-template/tree/master)
-->

This project was build upon the [scikit-learn template](http://contrib.scikit-learn.org/project-template/) in order to be compatible with the scikit-learn pipelines and (hyper)parameter search, while facilitating testing (including some API compliance), documentation, open source development, packaging, and continuous integration.

## Installation and Usage
This module is strictly related with the glcr module, this is why it is provided as submodule. To clone `digitaldna` and its `glcr` submodule, execute:
```shell
$ git clone --recurse-submodules <PREFIX-URL>/ddna-toolbox.git
```
for example:

```shell
$ git clone --recurse-submodules http://ci-repository.internal/wafi-ci/ddna-toolbox.git
```
Before installing the module you may need to install some more dependencies. After
doing that, you can install `glcr` by executing from project root (default: ddna-toolbox/):
```shell
$ pip install lcs_module/.
```
Then you can install `digitaldna` as:
```shell
$ pip install .
```
If the installation is successful, and `digitaldna` is correctly installed,
you should be able to execute the following in Python:
```python
from digitaldna.lcs import LongestCommonSubsequence
X = ['banana', 'ananan', 'anana', 'hanoi', 'banas']
estimator = LongestCommonSubsequence()
estimator.fit_predict(X)
```

## Getting started
Some usage examples can be found in the documentation website.

## Testing
To run a single unit test (e.g. test_lcs)
```
nosetests -v digitaldna.tests.test_lcs
```
To run all unit tests
```
nosetests -v .
```
from the project root.

## Important Links
- [Social Fingerprinting: Detection of Spambot Groups Through DNA-Inspired Behavioral Modeling](	https://ieeexplore.ieee.org/document/7876716)
- [Exploiting Digital DNA for the Analysis of Similarities in Twitter Behaviours](https://ieeexplore.ieee.org/document/8259831)
- [Linear Time Algorithms for Generalizations of the Longest Common Substring Problem](https://link.springer.com/article/10.1007/s00453-009-9369-1)
- [Scikit-learn Template Documentation](http://contrib.scikit-learn.org/project-template/)

## Contributing
If you want to contribute you can refer to the scikit-learn template documentation:
 - [scikit-learn template homepage](http://contrib.scikit-learn.org/project-template/)
 - [scikit-learn template source code](https://github.com/scikit-learn-contrib/project-template)
 - [scikit-learn Contributing section](http://scikit-learn.org/stable/developers/contributing.html)