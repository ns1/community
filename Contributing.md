At NS1, it makes us very happy to get pull requests, and we appreciate the time
and effort it takes to put one together. Below are a few guidelines that can
help get your pull request approved and merged quickly and easily.

First, if you are working on behalf of an existing NS1 client, we ask that you
raise your issue(s) via one of our support channels (email or NS1 Help Center)
before, or at least concurrent with, opening issues and PRs via Github. This
allows us to keep the right people and the right teams in the loop, and will
help us prioritize and respond effectively. Knowing that a PR is coming in
advance can help us budget time and people in advance, so we can get things
sorted fast!

It's important to note that the guidelines are recommendations, not
requirements. You may submit a pull request that does not adhere to the
guidelines, but ideation and development may take longer or be more involved.

* Avoid getting nitpicked for basic formatting. Match the style of any given
  file as best you can - tabs or spaces as appropriate, curly bracket
  placement, indentation style, line length, etc. If there are any linters
  mentioned in docs or Makefile, please run them.

* Avoid changes that have any possibility of breaking existing uses. Some of
  these codebases have many of users, doing creative things with them. Breaking
  changes can cause significant challenges for other users. It's important to
  note that some projects are dependencies of other projects, and changes may
  require cross-code base coordination. It can be challenging to identify if a
  small change will have large ramifications, so we mainly ask that you keep
  this in mind when writing or modifying code. Do your best to preserve
  interfaces, and understand that NS1 may need to reject pull requests if they
  would jeopardize platform stability or place an undue burden on other users.

* If there are unit and/or integration tests, keeping the test suites passing
  is a must before we can merge. And nice tests around the changes will
  definitely help get a patch merged quickly.

* Ensure that any documentation that is part of the project is updated as part
  of the pull request. This helps to expedite the merge process.

* Be considerate when introducing new dependencies to a project. If a new
  dependency is necessary, try to choose a well-known project, and to pin the
  version as specifically as possible.
