Best Practices
==============
Our guidance on how to best program together.
**These are suggestions, not rules.**
Strive to understand them, ignore them when necessary, ask when in doubt.

General
-------

* Don't duplicate the functionality of a built-in library.
* Don't swallow exceptions or "fail silently."
* Don't write code that guesses at future functionality.
* [Exceptions should be exceptional].

[Exceptions should be exceptional]: http://softwareengineering.stackexchange.com/a/184696

Object-Oriented Design
----------------------

* Avoid global variables.
* Avoid long (4+) parameter lists.
* Limit the collaborators of an object (entities an object depends on).
* Limit an object's dependencies (entities that depend on an object).
* [Prefer composition over inheritance].
* Prefer small methods. Between one and five lines is best.
* Prefer small classes with a single, well-defined responsibility. When a
  class exceeds 100 lines, it may be doing too many things.
* [Tell, don't ask].

[Prefer composition over inheritance]: https://robots.thoughtbot.com/reusable-oo-composition-vs-inheritance
[Tell, don't ask]: http://robots.thoughtbot.com/post/27572137956/tell-dont-ask

Git
---
* Don't push directly to master, instead open a pull request, even if you're going to merge it
  without review.
* Squash your commits before merging into master. You can use Github's *Squash and Merge* button or
  `git rebase -i` locally, to ensure that only atomic, descriptive commits go into the history of
  `master`.
* When staging changes, use `git add -p`, aka [patch mode]

[patch mode]: http://nuclearsquid.com/writings/git-add/

Ruby
----
* Avoid optional parameters. Does the method do too much?
* Avoid monkey-patching.
* Prefer classes to modules when designing functionality that is shared by multiple models.

Javascript
----------
* We agree with most things in the Airbnb guide: https://github.com/airbnb/javascript

