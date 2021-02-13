
![W3C Logo](https://www.w3.org/Icons/w3c_home)

# JSON-LD 1.1*

This is the repository describes extensions to [JSON-LD 1.1][], [JSON-LD 1.1 API][], and [JSON-LD 1.1 Framing][] to support triples as node identifiers as defined by [RDF-star]
developed by the [JSON for Linking Data Community Group](https://www.w3.org/community/json-ld/). The editors’ draft of the Note can also be [read directly](https://json-ld.github.io/json-ld-star/).

The JSON-LD-star Test Suite is a set of tests that can
be used to verify JSON-LD Processor for the RDF-star extensions to JSON-LD.

More information and an RDFS definition of the test vocabulary can be found at [vocab](https://w3c.github.io/json-ld-api/tests/vocab).

## General instructions for running the JSON-LD Test suites

Tests are run broadly the same as those for the core JSON-LD test suite, with the addition of the `rdfstar` option set to `true` for each test. If not set, explicitly, the test checks for proper behavior when not operating in RDF-star mode.

## Running tests

The top-level [manifest](manifest.jsonld) references the specific test manifests, which in turn reference each test associated with a particular type of behavior.

Implementations create their own infrastructure for running the test suite. In particular, the following should be considered:

* For JSON-Ld-star tests, the `specVersion` is set to `JSON-LD-star`.
* Some tests may have a `requires` property, indicating some optional behavior described by a test vocabulary term. Tests that use JSON-LD-star functionality have `"requires": "JSON-LD-star"` specified.

## Contributing Tests

If you would like to contribute a new test or a fix to an existing test,
please follow these steps:

1. Notify the JSON-LD Community mailing list, public-linked-json@w3.org,
   that you will be creating a new test or fix and the purpose of the
   change.
2. Clone the git repository: git://github.com/json-ld/json-ld-star.git
3. Make your changes and submit them via github, or via a 'git format-patch'
   to the [JSON-LD Community Group mailing list](mailto:public-linked-json@w3.org).

## Distribution

Distributed under the [W3C Test Suite License](http://www.w3.org/Consortium/Legal/2008/04-testsuite-license). To contribute to a W3C Test Suite, see the [policies and contribution forms](http://www.w3.org/2004/10/27-testcases).

## Disclaimer

UNDER THE EXCLUSIVE LICENSE, THIS DOCUMENT AND ALL DOCUMENTS, TESTS AND SOFTWARE THAT LINK THIS STATEMENT ARE PROVIDED "AS IS," AND COPYRIGHT HOLDERS MAKE NO REPRESENTATIONS OR WARRANTIES, EXPRESS OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, NON-INFRINGEMENT, OR TITLE; THAT THE CONTENTS OF THE DOCUMENT ARE SUITABLE FOR ANY PURPOSE; NOR THAT THE IMPLEMENTATION OF SUCH CONTENTS WILL NOT INFRINGE ANY THIRD PARTY PATENTS, COPYRIGHTS, TRADEMARKS OR OTHER RIGHTS.
COPYRIGHT HOLDERS WILL NOT BE LIABLE FOR ANY DIRECT, INDIRECT, SPECIAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF ANY USE OF THE DOCUMENT OR THE PERFORMANCE OR IMPLEMENTATION OF THE CONTENTS THEREOF.

## Code of Conduct

W3C functions under a [code of conduct](https://www.w3.org/Consortium/cepc/).

[RDF-star]:                 https://w3c.github.io/rdf-star/rdf-star-cg-spec.html
[JSON-LD 1.1]:          https://w3.org/TR/json-ld11
[JSON-LD 1.1 API]:      https://w3.org/TR/json-ld11-api
[JSON-LD 1.1 Framing]:  https://w3.org/TR/json-ld11-framing