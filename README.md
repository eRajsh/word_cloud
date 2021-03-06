[![licence](http://img.shields.io/badge/licence-MIT-blue.svg?style=flat)](https://github.com/amueller/word_cloud/blob/master/LICENSE)
[![DOI](https://zenodo.org/badge/21369/amueller/word_cloud.svg)](https://zenodo.org/badge/latestdoi/21369/amueller/word_cloud)

|      | Linux                                        | macOS                                        | Windows                                      |
|------|----------------------------------------------|----------------------------------------------|----------------------------------------------|
| PyPI | [![CircleCI][circleci_image]][circleci_link] | [![TravisCI][travisci_image]][travisci_link] | [![AppVeyor][appveyor_image]][appveyor_link] |

[circleci_link]: https://circleci.com/gh/amueller/word_cloud/tree/master
[circleci_image]: https://circleci.com/gh/amueller/word_cloud/tree/master.svg?style=svg

[travisci_link]: https://travis-ci.org/amueller/word_cloud
[travisci_image]: https://travis-ci.org/amueller/word_cloud.svg?branch=master

[appveyor_link]: https://ci.appveyor.com/project/amueller/word-cloud/branch/master
[appveyor_image]: https://img.shields.io/appveyor/ci/amueller/word-cloud/master.svg

text_cloud
==========

A little text cloud generator in Python, that generates a cloud of sentences from a list of sentences given as ain input. This is based on the nifty package from AMueller's, the wordcloud. Read more about the wordcloud package on the [blog
post][blog-post] or the [website][website].

The code is tested against Python 2.7, 3.4, 3.5, 3.6 and 3.7.

## Installation

If you are using pip:

    pip install textcloud




#### Installation notes

textcloud depends on `numpy` and `pillow`.

To save the textcloud into a file, `matplotlib` can also be installed. See [examples](#examples) below.

If there are no wheels available for your version of python, installing the
package requires having a C compiler set up. Before installing a compiler, report
an issue describing the version of python and operating system being used.


## Examples

Check out [examples/simple.py][simple] for a short intro. A sample output is:

![Constitution](examples/constitution.png)

Or run [examples/masked.py][masked] to see more options. A sample output is:

![Alice in Wonderland](examples/alice.png)

Getting fancy with some colors:
![Parrot with rainbow colors](examples/parrot_new.png)

Generating wordclouds for Arabic:

![Arabic wordlcloud](examples/arabic_example.png)





## Licensing
The textcloud library is MIT licenced, but contains DroidSansMono.ttf, a true type font by Google, that is apache licensed.
The font is by no means integral, and any other font can be used by setting the ``font_path`` variable when creating a ``TextCloud`` object.
