---
layout: post
title: SonarQube automates craftsmanship
subtitle: if you only dare to
---

A while ago I wrote a series on [SonarQube][sonar-qube] which is some sort of code analysis facility. You, dear reader, can find it [here][sonar-series], on the website of the [company][pragmasoft] I contracted for at the time of writing this article. Although the referenced article elaborates thoroughly on the subject, here I give a little summary.

SonarQube reinforces your daily development with static code analysis, the results of which feed linters and various issue harvesters. And it does it often, on a daily basis or on every commit (the harvesters). Or even instantly when you write code (the IDE linter called [SonarLint][sonar-lint]). Next, the harvesters upload the results to the SonarQube server for the analytical purpose: metrics, history recording, filterable visualizations, queryable code insights and lots more. And a wealth of plugins to enter the stage.

Present-day CI standards allow for plugging code tools into pipelines. For the eventual code package result be reliable in terms of various code quality metrics. SonarQube lets you define a set of thresholds and apply it onto a group of software projects. So then, every pipeline would fail if the project code doesn't meet the agreed requirements. What is more, by making use of merge/pull request issue reporting you can make code reviewer life easier. How - you ask? The pull request review screen would contain issue indicators pinned directly to particular lines of code being reviewed.

[Article 1][article-1] serves you a short introduction to the SonarQube facility and theoretical rationale behind. [Article 2][article-2], on the other hand, brings an entirely practical guideline on how to setup an end-to-end project analysis in .NET tech stack. [Article 3][article-3] zooms in on analysis results of Google .NET projects by one of the top-notch .NET developers Jon Skeet ([@jonskeet][skeet-twitter]). Complementary [Article 4][article-4] examines various properties of SonarQube thoroughly.

A little endeavour could bring a substantial long-term value. Providing you dare to set off on the journey. This might lead you to uncover painful truth about your codebase or development process (often both). However, as with many truth-based things, it has potential to gradually cure development hassle and reduce waste in the long run.

[article-1]: http://blog.pragmasoft.pl/software/2018-10-10-sonarqube-1-intro/ "Introduction to SonarQube"
[article-2]: http://blog.pragmasoft.pl/software/2018-10-10-sonarqube-2-setup-environment/ "Configuring SonarQube project analysis in .NET stack"
[article-3]: http://blog.pragmasoft.pl/software/2018-10-10-sonarqube-3-crushing-jon-skeets-code/ "Sample analyze of .NET projects by Jon Skeet"
[article-4]: http://blog.pragmasoft.pl/software/2018-10-24-sonarqube-4-project-analysis-details/ "Various aspects of SonarQube facility"
[pragmasoft]: https://pragmasoft.pl "Pragmasoft Sp. z o.o. company website"
[skeet-twitter]: https://twitter.com/jonskeet "Jon Skeet on Twitter"
[sonar-lint]: https://www.sonarlint.org/ "SonarLint IDE extension"
[sonar-qube]: https://www.sonarqube.org "SonarQube code analysis facility"
[sonar-series]: http://blog.pragmasoft.pl/software/2018-10-10-sonarqube-1-intro/ "SonarQube series, episode 1."
