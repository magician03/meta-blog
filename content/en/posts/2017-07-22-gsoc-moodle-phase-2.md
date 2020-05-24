+++
title = "GSoC’17 Journal: Phase 2"
description = ""
tags = [
    "gsoc",
    "moodle",
    "internship"
]
date = "2017-07-22"
categories = [
    "GSoC",
]
menu = "main"
+++

With Phase 2 of GSoC'17 about to end, it's time to recapitulate the work done during this period. Phase 2 has started on 30th June and ends on 24th July, approximately 3 weeks.

### Travis build optmization

With increasing number of tests the Travis build is timing out (50 min hard timeout) and this became main problem. The entire Travis Build process is then reconfigured, now it uses job matrix with 7 jobs. Each job is taking ~30-40 min to complete. The Node packages are also now cached in the build. This effectively reduces the enviroment setup internally inside Travis by 5 min for each job(quite valuable!).

### E2E Documentation draft

Existing documentation for E2E testing is outdated. The new improved Documentation is drafted and is 80% done. It now allows users to perform the E2E testing in the 3 different setups. The official Moodle Docs will be updated in Final Phase.

### Improved TestSuites
Some tests which can be easily improved/optimised are updated.All the tests are now working w.r.t integration branch(up-to-date Mobile Team development workflow). Rest will be improved in Final Phase.

### New TestSuites
New TestSuites have been added to test new functionalities of the App. Lesson, Feedback, Database, User profiles, CourseOverview and other resource modules are few of these.

### Progress Recap

#### Work done to date
* All the existing test suites are corrected
* New test suites for new activities/features have been added
* All are passing in Travis CI and SauceLabs browsers
* E2E documentation is 80% done
* Travis build greatly optimised by generating build matrix (7 jobs currently) and caching the node packages

#### Yet to do
*  Minor updates & Publish the documentation
*  Update the test suites to test new features in various activities and other new features

### Current Stats

* 143 E2E Tests
* 36 Test Suites
* 3hr 45min of actual Travis Build/Test time
* 40 min Travis Build/Test time after optimization
* 7 Travis jobs
* 39 Git commits

### Few related Links
* [Git branch for the GSoC'17 work](https://github.com/magician03/moodlemobile2/tree/gsoc2017)
* [Travis Build History for MoodleMobile2 Build & Testing](https://travis-ci.org/magician03/moodlemobile2/builds)
* [E2E Documentation draft](https://docs.google.com/document/d/1H7nQVvkYySftJX16dycBNdoK1xFRQN0MUsnvzUv6eJc/edit?usp=sharing)