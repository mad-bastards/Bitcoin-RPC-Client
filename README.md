# Bitcoin::RPC::Client - Bitcoin Core RPC client as a PERL module

This module implements in PERL the functions that are currently part of the
Bitcoin Core RPC client calls (bitcoin-cli).The function names and parameters
are identical between the Bitcoin Core API and this module. This is done for
consistency so that a developer only has to reference one manual:
https://bitcoin.org/en/developer-reference#getinfo

Currently only tested against Bitcoin Core v0.12.1.

DEPENDENCIES:
   - Moo
   - JSON::RPC::Client

INSTALL:
   - perl Makefile.PL
   - make
   - make test
   - make install

CAVEATS:
   - boolean parameters must be passed as JSON::true
   - fees are set server side (bitcoin.conf)

TODO:
   - Parse JSON error string
   - Implement support for fees
   - Documentation
