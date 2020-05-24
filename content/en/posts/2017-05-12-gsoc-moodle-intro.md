+++
title = "GSoC'17 Journal: Moodle Mobile - Project Proposal"
description = ""
tags = [
    "gsoc",
    "moodle",
    "internship"
]
date = "2017-05-12"
categories = [
    "GSoC",
]
menu = "main"
+++


First of all, I would like to thank my GSoC mentor Juan Leyva, Moodle Mobile Team members Daniel Palou, Pau Ferrer for their continuous help and support, Moodle's GSoC admin David Mudrak for all the guidance.


## Moodle & Moodle Mobile

Moodle is the world largest and most loved open-source Learning Management System(LMS). Moodle Mobile is the official mobile app for Moodle which brings the browser-based services of Moodle to Mobile devices across Android and iOS.

#### Some quick stats about Moodle & Moodle Mobile
- World largest and best Learning Management System / EdTech
- 100 Million+ (registered) weekly active users of Core Services
- ~10 Million downloads of Mobile App (Android & iOS)
- 234 countries, ~100 + Lang translations
- Open Source since 2002, kind of legacy codebase, high entry barriers for noobs to collaborate
- Used in Schools, Universities, Corporates, Institues, by Teachers, Students, Learners, Educators, Trainers etc
- Participating in GSoC since 2006


## Collaboration

My collaboration with Moodle Mobile began in December 2016 when I have sent a mail, out of blue, regarding one of the then-potential-project which I am interested to contribute. It was later dropped and Juan Leyva (Moodle Mobile Team Lead) encouraged me to look up into Mobile Tracker for other issues which would interest me. Since then I am actively contributing in Moodle Mobile and resolved some critical bugs and also added new features. Some of them are : 
* [MOBILE-1512](https://tracker.moodle.org/browse/MOBILE-1512) Add Module Prefetch Info in Context Menu for all Modules 
* [MOBILE-1157](https://tracker.moodle.org/browse/MOBILE-1157) Add Title, Description in all Resource Modules from Module Prefetch
* [MOBILE-1789](https://tracker.moodle.org/browse/MOBILE-1789) Add Message Search functionality via WebServices
* [MOBILE-1955](https://tracker.moodle.org/browse/MOBILE-1955) Increase the size & padding of some icons 
* [MOBILE-2050](2050) Modify the `font-size` of headlines in `.item mm-format-text`
* [MOBILE-1843](https://tracker.moodle.org/browse/MOBILE-1843) Quick fix for Dev Env Setup failure, Appium Issue
* [MOBILE-2095](https://tracker.moodle.org/browse/MOBILE-2095) Minor Code refactoring for sorting functionality.

Besides these, I have also tested some issues and participated in resolving other issues. All my Moodle development activity can be viewed in my Tracker profile [here](https://tracker.moodle.org/secure/ViewProfile.jspa?name=magician03).


## GSoC Project - [Improve End-to-End Testing in the Mobile App](https://docs.google.com/document/d/1zRKzCcvDpdhbIhteiyk4ctNOdinup-RahKclaGZHb4w/edit?usp=sharing)

#### Project Description
The project aims to enable the Moodle Mobile App with fully automated End-to-End testing capabilities with SauceLabs and Travis CI using latest upgraded versions of Node, Protractor, Gulp, Appium, Selenium with latest Moodle Mobile App v3.3.0 [~15/5/2017].

Integrating SauceLabs and TravisCI enables a completely automated build on Travis along with End-to-End testing on SauceLabs’ Browsers, Mobile/Tablet Android Emulators, Mobile/Tablet iOS Simulators [and Real Devices exclusively for premium users]. Incase of any failure in Travis build, debugging can be easily done as SauceLabs provides the actual video and screenshot logs of all the tests for 30 days [only metadata & screenshots after that] and TravisCI restores the build log for lifetime of a repository.

#### Project Goals
- Upgrade Node, Protractor, Gulp, Appium, Selenium and other related dependencies
- Configure the App for Travis build and SauceLabs testing via Travis
- Fix all the failing E2E tests
- Add E2E tests for newly added features/modules in Moodle Mobile v3.1.x, v3.2.x, v3.3.0
- Modify the existing documentation of Moodle Mobile Development Environment Setup and End-to-End testing environment



Finally, I am very excited to be a part of such large organisation with global appeal and being the sole GSoC selection, a bit tensed too. However, with the very helpful, supportive Dev Team I am confident and optimistic. Looking forward for great experiences this summer 2017.
