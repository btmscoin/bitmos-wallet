# Bitnow Core integration/staging repository

[![Build Status](https://api.travis-ci.org/bitnows/bitnow.svg?branch=master)](https://travis-ci.org/bitnows/bitnow) ![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg)

## What is Bitnow?

Bitnow (BNOW) is a sustainable cryptocurrency modeled after Satoshi Nakamoto’s vision for Bitcoin. 
It is a decentralized, peer-to-peer transactional currency designed to offer a solution to the problem posed by the exponential increase in energy consumed by Bitcoin and other proof-of-work currencies. 
Proof-of-work mining is environmentally unsustainable due to the electricity used by high-powered mining hardware.
Bitnow utilizes the Tier Protocol, an energy efficient proof-of-stake algorithm inspired by PIVX/DASH, can be mined on any computer, and will never require specialized mining equipment. 
The Tier Protocol offers a simple solution to Bitcoin sustainability issues and provides a faster, more scalable blockchain that is better suited for daily transactional use.
Fast transactions featuring guaranteed zero confirmation transactions, we call it SwiftTX.
Decentralized blockchain voting providing for consensus based advancement of the current Masternode technology used to secure the network and provide the above features, each Masternode is secured with a collateral of 1,000,000 BNOW.

- Fast transactions featuring guaranteed zero confirmation transactions, we call it _SwiftTX_.
- Decentralized blockchain voting providing for consensus based advancement of the current Masternode
  technology used to secure the network and provide the above features, each Masternode is secured
  with a collateral of 100,000  BNOW.


Please reach out at Bitnow. bitnow.team@gmail.com


Bitnow Core integration/staging repository
=====================================

Bitnow is a brand new digital currency that combines all the positive aspects of successful digital currencies, while taking into account their flaws and weak points.
The project brings tangible benefits not only to the digital world but also to the real one.


### Coin Specs

<table>
<tr><td>Name & ticker</td><td>BITNOW / BNOW</td></tr>
<tr><td>Consensus algorithm</td><td>POS</td></tr>
<tr><td>POS phase duration</td><td>600 blocks</td></tr>
<tr><td>POS block reward</td><td>200 BNOW</td></tr>
<tr><td>Instamine protection</td><td>First 600 blocks</td></tr>
<tr><td>Hashing algorithm</td><td>Keccak</td></tr>
<tr><td>Estimated Bitnow supply during POS</td><td>5,000,000,000 BNOW</td></tr>
<tr><td>POS starting block</td><td>2,001 block</td></tr>
<tr><td>POS phase duration</td><td>Unlimited</td></tr>
<tr><td>POS block reward distribution</td><td>SeeSaw</td></tr>
<tr><td>Premine</td><td>4,000,000,000 BNOW</td></tr>
<tr><td>Blocksize</td><td>1 MB</td></tr>
<tr><td>Blocktime average</td><td>1 min (DGW3)</td></tr>
<tr><td>Number of transaction confirmations</td><td>6</td></tr>
<tr><td>Maturity</td><td>288 confirmations</td></tr>
</table>


## License

BitGreen Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

## Development Process

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/bitnows/bitnow/tags) are created
regularly to indicate new official, stable release versions of BitGreen Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md)
and useful hints for developers can be found in [doc/developer-notes.md](doc/developer-notes.md).

## Testing

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