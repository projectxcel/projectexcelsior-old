NOTICE OF PROPRIETARY RIGHTS: Any blockchain initiated with the specific timestamp of 1637710944, nonce of 2085969695, difficulty target 
of 0x1e0ffff0, version number of 1, and a reward value of 50 * COIN, producing a Genesis Block hash of 
"0x94e01e42b72f879cb8db253ce2d74b749c338e73e428aff2bf6dd75db6ddf316" and a Merkle Root hash of "0xa507f271f981e998c341679be851c734c3b053c303589068b004f92e79e9d5fb" (collectively referred to as the "Identified Blockchain Parameters"), is hereby acknowledged as the proprietary property of Project Excelsior. The Identified Blockchain Parameters have been developed, maintained, and are the exclusive property of Project Excelsior.

Without the express written consent of Project Excelsior, no person, entity, or party has the right or license to use the Identified Blockchain Parameters for monetary gain, profit, or any form of economic advantage. Any such unauthorized use, reproduction, distribution, or other exploitation of the Identified Blockchain Parameters constitutes a violation of Project Excelsior's rights and may subject the violator to legal action, including, but not limited to, claims for damages, injunctive relief, and the recovery of costs and attorney's fees incurred in connection with the enforcement of Project Excelsior's rights.

Project Excelsior reserves all rights not expressly granted herein, and this Notice does not constitute any waiver of any rights that Project Excelsior may have, whether at law, in equity, or otherwise.







ProjectExcelsior Core integration/staging tree
=====================================

This is the original core for XCL. XCL has been updated to V0.21.2 (this aligns with Litecoin's latest update)

https://projectxcel.com

What is ProjectExcelsior?
----------------

ProjectExcelsior is an experimental digital currency that enables instant payments to
anyone, anywhere in the world. ProjectExcelsior uses peer-to-peer technology to operate
with no central authority: managing transactions and issuing money are carried
out collectively by the network. ProjectExcelsior Core is the name of open source
software which enables the use of this currency.

For more information, as well as an immediately useable, binary version of
the ProjectExcelsior Core software, see [https://projectxcel.com](https://projectxcel.com).

License
-------

ProjectExcelsior Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/projectexcelsior-project/projectexcelsior/tags) are created
regularly to indicate new official, stable release versions of ProjectExcelsior Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

The developer [mailing list](https://groups.google.com/forum/#!forum/projectexcelsior-dev)
should be used to discuss complicated or controversial changes before working
on a patch set.

Developer IRC can be found on Freenode at #projectexcelsior-dev.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](src/test/README.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`. Further details on running
and extending unit tests can be found in [/src/test/README.md](/src/test/README.md).

There are also [regression and integration tests](/test), written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/test) are installed) with: `test/functional/test_runner.py`

The Travis CI system makes sure that every pull request is built for Windows, Linux, and OS X, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
------------

We only accept translation fixes that are submitted through [Bitcoin Core's Transifex page](https://www.transifex.com/projects/p/bitcoin/).
Translations are converted to ProjectExcelsior periodically.

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.
# projectexcelsior
