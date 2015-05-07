
# Modern code development strategies

## Radovan Bast

Licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
Code examples: [OSI](http://opensource.org)-approved [MIT license](http://opensource.org/licenses/mit-license.html).

---

layout: false

## Version control

- No-brainer
- Mandatory for reproducible scientific results

---

## Test-driven development

- First write tests, then verify that tests fail, then write functionality until tests pass
- TDD avoids gold-plating
- Tests protect functionality
- Functionality without tests will break at some point
- Broken functionality: huge cost
- (Unit) tests are the most accurate documentation
- [Code coverage](https://testboard.org)

---

## Code review

- Traditional approach: "Please give me access to the main development line and I will program something and I promise not to break anything."
- Code review: "Here, I have programmed something. Please review and merge it to the main development line if you like it. The green badge shows that I did not break anything."
- Slower in the short-term, faster in the long-term
- Better quality code
- Allows to enforce a certain style/policy/philosophy
- Peer-review for code
- Efficient tool to learn
    - Programmer from the team
    - Team from the programmer
- Code review can be coupled with automatic testing and coverage analysis
- Git allows decentralized development

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

---

## Efficient issue tracking

- Use/generate ChangeLog
- Assign to yourself once you start working on it
- Use Milestones
- Public issues
- https://testboard.org
- Do not bugtrack in your head

---

## Simplify, simplify, simplify

- Avoid complexity
- Fear state
- Use functional programming style
- YAGNI
- Cut all dead wood
- Modularize or die
- Referential transparency

---

## Referential transparency

- Referential transparency

```python
def add_numbers(i, j):
    return i + j
```

- Referential opacity

```python
def get_num_page_visits():
    global num_page_visits
    num_page_visits = num_page_visits + 1
    return num_page_visits
```

- Referential transparency makes it easier to
    - Simplify
    - Optimize
    - Refactor
    - Memoize
    - Parallelize
    - Reuse
    - Test

---

## Human time vs CPU time

*"Programs aren't written for computers: they're written for other programmers who will have to integrate and maintain them."*
[C++ In Action: Industrial Strength Programming Techniques by Bartosz Milewski]

- Human time is more valuable than CPU time
- No SIXLTR variables
- No 72-6 character limit
- Pure functions
- Make your code readable and understandable by others
- Document what functions do
- If you cannot describe a function in one sentence, it is too complicated
- If the description contains "and", "or", "except", "also", it is too complicated
- If the function does not fit on one screen it is too complicated

---

## Single-core performance does not matter

- The slower code that scales catches the worm
- The slower language that scales catches the worm
- The slower algorithm that scales catches the worm
- Codes that scale get more grants
- Codes that scale get to run on modern supercomputers
- Codes that scale can utilize modern hardware architectures
- Functional programming

---

## Licensing

- Allow derived products
- Allow external contributions
- Simplify funding
- Standard licenses better than customized
- Compatibility is an issue (git submodules)

---

## Modern documentation

- Rendered using Sphinx
- Served via ReadTheDocs
- Update upon push (post-receive hook)
- Developer's manual
- Reply by doc

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

## Basis set repo

- Should be own repo
- Make it public
- JSON API (or some other standard API)
- Versionned

---

## Provide benchmarks

- Useful for proposals
- Useful for supercomputer support personnel
- Useful for hardware vendors
- Important for time tests

---

## Market success stories

- Nice images
- Image carousel
- Good for proposals
- Attract users
- Attract developers

---

## Training

- Modern code development tools and practices need to be part of the curriculum
  for students who program
