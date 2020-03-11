# Devops Study Guide

This Repository here has the collection of Books that you should read in order to have profound knowledge of Devops.The copyrights prevented me to upload the ebooks in here. However I have provided the links to buy these ebooks.

** Below are the list of study materials.**
---

1. Jenkins link : http://shop.oreilly.com/product/0636920010326.do
2. Gradle link: https://www.amazon.in/Gradle-Action-Benjamin-Muschko/dp/1617291307
3. Maven link: https://www.amazon.in/Maven-Definitive-Guide-ebook/dp/B002PEP4P0
4. Circle Ci link: https://circleci.com/docs/2.0/
5. GIt Lab link: https://www.amazon.com/GitLab-Repository-Management-Jonathan-Hethey-ebook/dp/B00GTQD5OC
6. Groovy link: https://www.amazon.in/Learning-Groovy-Adam-L-Davis-ebook/dp/B01JSUJHS8
7. AWS solution architect Associate link: https://www.amazon.com/Certified-Solutions-Architect-Official-Study-ebook/dp/B01M6W6WYD
8. AWS solution architect Professional link: https://www.amazon.com/AWS-Certified-Solutions-Architect-Professional/dp/1642499544
9. The Phoenix Project link:https://www.amazon.com/Phoenix-Project-DevOps-Helping-Business-ebook/dp/B00AZRBLHO

** FAQ  **
---

+ Continuous integration, continuous deployment, and continuous delivery are like vectors that have the  same direction, but different magnitude. Their goal is the same: make our software development and release process faster and more robust.
+ The key difference between the three is in the scope of automation applied. What gets people who are new to the field confused is that they are not mutually exclusive, but include each other, like Russian dolls.
+ Most developers start with Continuous Integration (CI), which is about everyone merging code changes to a central repository multiple times a day. Each merge triggers an automated build and testing sequence for the given project.Depending on the programming language, the program may first need to be compiled. Today there is also an increasing need to package the code in a Docker container. Automated tests then verify specific units of code, UI behavior, application performance, API reliability, and more. Together, all these steps are commonly referred to as the “Build” stage.CI acts as a safety net that lets developers prevent many issues before they reach users. As a result, developers ship code with more confidence, but not necessarily faster — the deployment process may still be manual, long, and error-prone. The best initial investment developers can make is to ensure that their automated test suite is comprehensive and stable enough that they feel safe to deploy every passed CI build to a staging, and later production environment, without a long manual QA (quality assurance) process.

+ Continuous integration involves a series of steps that are automatically performed to integrate code from multiple sources, create a build and test. Each time a build or a set of code passes the tests, it’s automatically deployed out to a staging environment where further testing such as load testing and manual exploratory testing is conducted. This process can be repeated for days depending upon the project delivery requirements.

+ Wikipedia describes Continuous Integration (CI) as “the practice of merging all developer working copies to a shared mainline several times a day.” The CI Model takes Agile a step further by automating the integration and Testing.

+ The thought of integrating new code with the mainline of the application code several times a day can be a scary thought for those more familiar with the waterfall methodology. At a glance, it seems that this would be massively problematic, resulting in the introduction of numerous bugs into the mainline code. However, as the majority of development teams have already discovered, the result is quite the opposite. The code segments being worked on at any given time are much smaller and are therefore easier to both code and debug if there is an issue. So, unlike the waterfall methodology where you create an entire version of the application and then submit it for testing, with continuous integration, the developer submits only small segments of the application at a time. Each of these code segments is then saved and automatically sent to the build server either immediately, or at regular intervals throughout the day. The build is then automatically passed to a test server that executes a series of automated unit tests to ensure that the new code segments work as planned. For additional information on the CI framework, Gartner has published a great article called, “A Guidance Framework for Continuous Integration: The Continuous Delivery ‘Heartbeat,” by Bill Holz and Sean Kenefick.By doing this, the new code segments are built, integrated and tested in mere minutes, providing the developer with immediate feedback on the status of the code and any related issues.

+ Key Strengths of Continuous Integration (CI) Testing
It’s no secret that testing the same test scripts every day can be a highly monotonous duty. Most development teams have found that the automation of test scripts wherever possible goes a long way. Not to mention, it also provides immediate feedback to the developer in mere minutes.
    - Issue Resolution: When the automated test scripts do find an issue in the code, because the code  segments are small, the developers have been able to make quick work of issue identification and resolution.

    - Phased Changeover: With small iterative changes, studies have confirmed that the migration from an old version of the software to a newer version is much easier because the users are eased into the changes, instead of having to learn a new version of the software all at once.

    - Improved Team Morale: Surprisingly, submitting these iterative changes has also improved dev team morale, especially when tasked on larger projects. The reason is that it’s part of our human nature that we like to see accomplishments regularly. Unlike the waterfall methodology, where a large project can drag on for weeks or even months without completing any key milestones, the iterative approach allows developers to achieve multiple milestones per day. This also provides the immediate gratification of seeing their code passing the automated tests several times a day.

    - Increased Velocity: Teams have found that with the iterative changes to the code, automated builds, automated testing, and the rapid identification of issues, the overall velocity of the project delivery is significantly faster in comparison to waterfall methodology.

    - Improved Quality:
    Because issues are found and resolved with each sprint, those larger, more comprehensive development issues are substantially mitigated. This is because once a sprint has been deployed, subsequent code iterations are then added to the code that has already been proven to be functionally correct. This eliminates the issue of needing to fix multiple incorrectly developed modules because of a coding issue in a single module.

    - Improved Budget:
    With the increase in delivery velocity and shifting the identification and resolution of coding issues left, teams are saving a lot of time and resources, which all add up to a healthier bottom line.

+ In continuous deployment, every change goes through an automated pipeline and a working version of the application is automatically pushed to production. It does not involve any release approval cycle and the project teams need to ensure that every time a code is updated, tested and released, it works smoothly at the customer’s end. Naturally, a lot depends on the quality of the test suite. With continuous deployment, teams can have multiple software deployments on any given day and don’t have to sweat about a major release

+ Continuous Deployment is a step up from Continuous Delivery in which every change in the source code is deployed to production automatically, without explicit approval from a developer. A developer’s job typically ends at reviewing a pull request from a teammate and merging it to the master branch. A CI/CD service takes over from there by running all tests and deploying the code to production, while keeping the team informed about outcome of every important event.

+ Continuous deployment takes a further step from continuous delivery. It is a software engineering practice that ensures code changes are continuously released into the production environment. The goal is to release a new version whenever developers make changes and automatically get those changes to the end users. 

+ Continuous deployment is the ultimate goal of software development companies. Your company’s development and IT teams must properly prepare to tackle implementing continuous deployment. Production-ready environments and appropriate practices must be put in place to make sure the live environment is up to par. 

+ In continuous deployment, codes are run and maintained in a simulated environment, ensuring that the ultimate quality is taken into consideration. Real-time monitoring of the live environment is also a requirement to keep track of any arising issues and resolve them quickly. 