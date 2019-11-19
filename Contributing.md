At NS1, It makes us very happy to get Pull Requests, and we respect and
appreciate the time and effort it takes to put one together. We will do our
best to be communicative and help out with them. That said, there are a few
guidelines that can help get your Pull Request approved and merged quickly
and painlessly, with a minimum of fuss.

First, if you are working on behalf of an existing NS1 client, we ask that you
raise your issue(s) via regular channels before, or at least concurrent with,
opening issues and PRs via Github. This allows us to keep the right people
and the right teams in the loop, will help us prioritize and respond
effectively. Knowing that a PR is coming in advance can help us budget time and
people in advance, so we can get things sorted fast!

These are guidelines and you are welcome to submit a Pull Request that does not
follow them. If the idea is sound and the code is good, but does not follow
these guidelines, we will likely be happy to to discuss and get things into
shape ourselves, but it may take some time.

* Avoid getting nitpicked. Match the style of any given file as best you can,
  i.e. tabs or spaces as appropriate, curly brace placement, indentation style,
  line length, etc... If there are any linters mentioned in docs or Makefile,
  please run them. In general, better to fit in than to be correct.

* Avoid changes that have any possibility of breaking existing uses. Many of
  these codebases have lots of users, doing creative things, and breaking
  changes can be a real pain for them. Some projects are also relied on by
  higher-level projects, both internal and external, and sometimes coordinating
  even minor changes can be tricky.
  It can be a challenge to identify when a small change can have large
  ramifications, so we mainly ask that you keep this in mind when writing code.
  Do your best to preserve interfaces, and be understanding if we cannot accept
  good work due to our responsibility to keep things stable, and to avoid
  breakage that may not be obvious at all.

* If there are unit and/or integration tests, keeping the test suites passing
  is a must before we can merge. And nice tests around the changes will
  definitely help get a patch merged quickly.

* Ensuring that any documentation that is part of the project is updated per
  changes will help get Pull Requests merged quickly. We call this out because
  it is easy to forget!

* Be considerate when introducing dependencies. It's often pretty clear from
  looking at existing dependencies whether a new dependency will be
  controversial or not worth mentioning. Where possible, pin dependencies as
  specifically as possible.
