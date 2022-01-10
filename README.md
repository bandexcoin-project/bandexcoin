![alt text](https://bandexcoin.com/wp-content/uploads/2021/08/image-readme-github.png)

Bandexcoin Core integration/staging tree
=====================================

Website : https://bandexcoin.com <br />
Explorer : http://explorer.bandexcoin.com/ <br />
Pool : https://mining.bandexcoin.com/ <br />
Forum : https://bandexcoin.com/community <br />

The specifications are: <br />
Name: Bandexcoin <br />
Ticker: BEX <br />
First letter: B (or M) <br />
Maturity: 100 <br />
Max supply: 81,919,998 <br />
P2p port: 6333 <br />
Rpc port: 6332 <br />
Halving: 512,000 <br />
Block time: 5 min <br />
Diff time: 576 blocks <br />
Block reward: 80 <br />
Premined: 0 <br />
Algo: scrypt <br />

Discord : https://discord.gg/7etm8J9xyc <br />
Telegram : https://t.me/joinchat/u5uqY0ytVzg5NGE8 <br />
Reddit : https://www.reddit.com/r/bandexcoin <br />
Twitter : https://twitter.com/bandexcoin <br />
Youtube : https://www.youtube.com/channel/UCWnFcK_ShvD69G50_fv-jpg <br />
Facebook : https://www.facebook.com/profile.php?id=100071631310427 <br />
Instagram : https://www.instagram.com/bandexcoin/

What is Bandexcoin?
----------------

Bandexcoin is an experimental digital currency that enables instant payments to
anyone, anywhere in the world. Bandexcoin uses peer-to-peer technology to operate
with no central authority: managing transactions and issuing money are carried
out collectively by the network. Bandexcoin Core is the name of open source
software which enables the use of this currency.

For more information, as well as an immediately useable, binary version of
the Bandexcoin Core software, see [https://bandexcoin.com](https://bandexcoin.com).

License
-------

Bandexcoin Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/bandexcoin-project/bandexcoin/tags) are created
regularly to indicate new official, stable release versions of Bandexcoin Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md)
and useful hints for developers can be found in [doc/developer-notes.md](doc/developer-notes.md).

The developer [mailing list](https://groups.google.com/forum/#!forum/bandexcoin-dev)
should be used to discuss complicated or controversial changes before working
on a patch set.

Developer IRC can be found on Freenode at #bandexcoin-dev.

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

The Travis CI system makes sure that every pull request is built for Windows, Linux, and macOS, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
------------

We only accept translation fixes that are submitted through [Bitcoin Core's Transifex page](https://www.transifex.com/projects/p/bitcoin/).
Translations are converted to Bandexcoin periodically.

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.
