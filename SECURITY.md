# Security policy

## Reporting a vulnerability

Please **do not open a public issue** for a security problem.

Report it privately by either:

1. Using GitHub's **Report a vulnerability** button on the repository's Security tab (private vulnerability reporting), or
2. Emailing **info@zenxsys.com** with the subject "Security report" and the details below.

Please include:

- the repository and version (or commit) affected;
- a description of the issue and its impact;
- steps or a proof of concept to reproduce it;
- whether you believe it is already being exploited.

Do not include real credentials or customer data in a report.

## What to expect

- We aim to acknowledge your report within **three business days**.
- We aim to give you an initial assessment within **ten business days**, and to keep you updated until it is resolved.
- We will agree a disclosure date with you. We ask for a reasonable period to release a fix before details are made public, normally up to 90 days.
- We will credit you in the release notes if you wish, and we will not take legal action against good-faith research that follows this policy.

## Scope

In scope: the code in the repositories of this organisation.

Out of scope: the commercial ZenXPAM platform and Zenxsys websites. You can report issues with those to the same address and we will route them, but please do not test against systems you do not own or have permission to test.

## Supported versions

Security fixes are made to the latest released version of each repository. Please upgrade before reporting, if you can.

## Safe handling of secrets in these tools

These tools are designed to handle credentials. If you find any path where a secret value is printed, logged, written with permissive file modes, or included in an error message, please treat it as a security issue and report it privately.
