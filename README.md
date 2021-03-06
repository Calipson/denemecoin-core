denemecoin Core integration/staging tree
=====================================

http://denemecoin.org

What is denemecoin? 
----------------

denemecoin is a decentralized open source information registration and transfer system based on the Bitcoin cryptocurrency.

What does it do?
----------------

* Securely record and transfer arbitrary names (keys).
* Attach a value (data) to the names (up to 520 bytes, more in the future).
* Transact denemecoins, the digital currency (ℕ, DC).

denemecoin was the first fork of Bitcoin and still is one of the most innovative altcoins. It was first to implement merged mining and a decentralized DNS. denemecoin squares Zooko's Triangle!

What can it be used for?
----------------

* Protect free-speech rights online by making the web more resistant to censorship.
* Access websites using the .bit domain (with TLS/SSL).
* Store identity information such as email, GPG key, BTC address, TLS fingerprints, Bitmessage address, etc.
* Human readable Tor .onion names/domains.
* File signatures, Voting, bonds/stocks,/shares, web of trust, escrow and notary services (to be implemented).

~~For more information, as well as an immediately useable, binary version of~~
~~the denemecoin Core software, see https://denemecoin.org/?p=download.~~
Public binary downloads are not yet posted.

License
-------

denemecoin Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/Calipson/denemecoin-core/tags) are created
regularly to indicate new official, stable release versions of denemecoin Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

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

**Translation workflow is not yet set up for denemecoin Core.  For strings which are common to Bitcoin Core, see below.**

Changes to translations as well as new translations can be submitted to
[Bitcoin Core's Transifex page](https://www.transifex.com/projects/p/bitcoin/).

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.

Translators should also subscribe to the [mailing list](https://groups.google.com/forum/#!forum/bitcoin-translators).
