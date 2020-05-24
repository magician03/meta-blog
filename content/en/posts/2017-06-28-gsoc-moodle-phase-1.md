+++
title = "GSoC’17 Journal: Phase 1"
description = ""
tags = [
    "gsoc",
    "moodle",
    "internship"
]
date = "2017-06-28"
categories = [
    "GSoC",
]
menu = "main"
+++



With Phase 1 of GSoC'17 completed, it's now time to outline the work done during this period. Phase 1 has started on 30th May and ended on 26th June, approximately 3 weeks.

### Page Object Library

The page object library which is used to interact with the web page and test it was outdated. It is now updated with latest protractor features like `ExpectedConditions` , `wait`, `sleep` etc. This helped the testing in many ways, especially, as the app totally depends on Web Services calls and heavy Ionic and Angular rendering, it takes uncertain times to load the web pages. With the new improved library these problems are addressed well.

### Karma Unit Tests

Karma Unit tests which are written for premature version of the App are currently outdated and might be misleading for beginner contributors. Since there are no plans to add Unit Tests any time soon, they are safely removed along with its related karma dependencies.

### Travis-Sauce-Protractor Config files

Configuration files for Travis-Sauce-Protractor are written for Browser, Android, iOS. Android, iOS are to be via local machine with few number of tests at a time(as suace emulators, devices aren't restarting well often and are quite inconsistent). Browsers however work well and are relatively consistent with performance, so E2E testing is done SauceLabs via Travis. The Travis .yaml file is also updated accordingly and seprate config files are created for each purposes.


### Correction of E2E Test Suites

E2E tests which are present earlier are incorrect and are failing(thereby failing the Travis build). Also, there is a new course in the demo site 'Digital Literacy' added by MoodleHQ Team to exclusively test Mobile App features. So, all the course-specific tests are now corrected and migrated to that course. All other tests are also now corrected and passing the Travis build.

Here is the list of test-suites corrected : 
* `files.spec.js`
* `notes.spec.js`
* `calendar.spec.js`
* `contacts.spec.js`
* `participants.spec.js`
* `notification.spec.js`
* `coursecompletion.spec.js`
* `teacher_participation.spec.js`
* `label.spec.js`
* `login.spec.js`
* `survey.spec.js`
* `grades.spec.js`
* `courses.spec.js`
* `teacher_new_staff_induction_course.spec.js`
* `mod_book.spec.js`
* `mod_chat.spec.js`
* `resource.spec.js`
* `mod_wiki.spec.js`
* `settings.spec.js`
* `quiz.spec.js`
* `mod_forum.spec.js`
* `mod_assign.spec.js`
* `mod_choice.spec.js`
* `mod_folder.spec.js`
* `mod_glossary.spec.js`
* `teacher_course.spec.js`
* `teacher_grades.spec.js`
* `course_contents.spec.js`
* `course_filtering.spec.js`

### Few related links :
* [Git branch for the GSoC'17 work](https://github.com/magician03/moodlemobile2/tree/gsoc2017)
* [Travis Build History for MoodleMobile2 Build & Testing](https://travis-ci.org/magician03/moodlemobile2/builds)