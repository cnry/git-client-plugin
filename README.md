Utility plugin for Git-related support
======================================

Extracted from [git-plugin](https://wiki.jenkins-ci.org/display/JENKINS/Git+Plugin)
to make it easier for other plugins to use and contribute new features.

* see [Jenkins wiki](https://wiki.jenkins-ci.org/display/JENKINS/Git+Client+Plugin) for detailed feature descriptions
* use [JIRA](https://issues.jenkins-ci.org) to report issues / feature requests

Contributing to the Plugin
==========================

Plugin source code is hosted on [GitHub](https://github.com/jenkinsci/git-client-plugin).
New feature proposals and bug fix proposals should be submitted as
[GitHub pull requests](https://help.github.com/articles/creating-a-pull-request).
Fork the repository on GitHub, prepare your change on your forked
copy, and submit a pull request.  Your pull request will be evaluated
by the [Cloudbees Jenkins job](https://jenkins.ci.cloudbees.com/job/plugins/job/git-client-plugin/)
and you should receive e-mail with the results of the evaluation.

Before submitting your change, please assure that you've added a test
which verifies your change.  There have been many developers involved
in the git client plugin and there are many, many users who depend on
the git-client-plugin.  Tests help us assure that we're delivering a
reliable plugin, and that we've communicated our intent to other
developers in a way that they can detect when they run tests.

Code coverage reporting is available as a maven target and is actively
monitored.  Please try your best to improve code coverage with tests
when you submit.

Before submitting your change, please review the findbugs output to
assure that you haven't introduced new findbugs warnings.

To Do
=====

* Fix [bugs](https://issues.jenkins-ci.org/secure/IssueNavigator.jspa?mode=hide&reset=true&jqlQuery=project+%3D+JENKINS+AND+status+in+%28Open%2C+"In+Progress"%2C+Reopened%29+AND+component+%3D+git-client)
* Create infrastructure to detect [files opened during a unit test](https://issues.jenkins-ci.org/browse/JENKINS-19994) and left open at exit from test
* Create credential tests
* Create submodule tests
* Improve code coverage in current tests
* Improve javadoc
* Complete more of the JGit implementation
