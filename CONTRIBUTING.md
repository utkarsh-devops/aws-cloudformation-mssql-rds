Contributing to aws-cloudformation-mssql-rds
=======================

The easiest ways to contribute to `aws-cloudformation-mssql-rds` are:


  * Creating a new [issue].
  * Forking the repository, make your contribution and submit a pull request.
    See [Git Flow](#git-flow) for further information.

[issue]: https://github.com/utkarsh-devops/aws-cloudformation-mssql-rds//issues/new

Git Flow
--------
We chose to use the [Git flow branching model][flow] for `aws-cloudformation-mssql-rds`, so you are
kindly required to follow the same model when you make your contributions. This
basically means that:

  * If you are fixing a bug, you can create a *hotfix* branch from the affected
  release (preferably, the latest one) and send a pull request from that branch.
  * If you are creating a new feature, please checkout the `develop` branch and
  send a pull request from there.
  * I won't consider pull request coming from the `master` branch and if I do, I
    won't be quick.

[flow]: http://nvie.com/posts/a-successful-git-branching-model/

Coding Conventions and Style
----------------------------
CloudFormation's guide for syntax and general best practices are used. Check https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/gettingstarted.templatebasics.html for more info.

