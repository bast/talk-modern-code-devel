
# Modern code development strategies

## Radovan Bast

Licensed under CC BY 4.0.
Code examples: OSI-approved MIT license.

---

layout: false

## TDD

- Code coverage

---

## Code review

- Code review
- Decentralized development

---

## Basis set repo

- Should be own repo
- Make it public
- JSON API (or some other standard API)
- Versionned

---

## Licensing

- Allow derived products
- Allow external contributions
- Simplify funding
- Standard licenses better than customized
- Compatibility is an issue (git submodules)

---

## Training

- Write me

---

## Information flow: the issue with emails

- Emails get lost or overlooked
- Issues
    - Clear what issues are known
    - Clear who is working on it
    - Clear whether an issue is solved
    - Permanent (also future generations can follow them)
    - Easy to subscribe/unsubscribe to/from
    - Easy to involve people with @mentions
    - Easy to track
    - Do not get lost
    - Labels
    - Milestones
    - Auto-closing gives well defined lifetime

### Efficient issue tracking

- ChangeLog
- Milestones
- Public issues
- https://testboard.org

---

## Modern documentation

- Rendered using Sphinx
- Served via ReadTheDocs
- Update upon push (post-receive hook)
- Developer's manual
- Reply by doc

---

## Simplify, simplify, simplify

- Avoid complexity
- Fear state
- Use functional programming style
- Referential transparency
- YAGNI
- Avoid crypto-coding
- Cut all dead wood
- Modularize or die

---

## Semantic versioning

- We have many modules/libraries and dependencies and they evolve
- Given a version number MAJOR.MINOR.PATCH, increment the:
    - MAJOR version when you make incompatible API changes
    - MINOR version when you add functionality in a backwards-compatible manner
    - PATCH version when you make backwards-compatible bug fixes
- http://semver.org
- Example:
    - Library OpenRSP requires package Gen1Int
    - At the time that OpenRSP is created, Gen1Int is at version 3.1.0
    - We can safely specify the dependency as greater than or equal to 3.1.0 but less than 4.0.0
    - When Gen1Int version 3.1.1 and 3.2.0 become available, they will be compatible

---

## Human time vs CPU time

- Write me

---

## Single-core performance does not matter

- Write me

---

## Provide benchmarks

- Useful for proposals
- Useful for support personnel
- Useful for hardware vendors
- Important for time tests

---

## Market success stories

- Good for proposals
- Attract users
- Attract developers
- Image carousel
