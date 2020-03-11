# Devops Study Guide

This Repository here has the collection of Books that you should read in order to have profound knowledge of Devops.The copyrights prevented me to upload the ebooks in here. However I have provided the links to buy these ebooks.

**Below are the list of study materials.**
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

**Continuous Integration (CI)**
---

+ Continuous integration, continuous deployment, and continuous delivery are like vectors that have the  same direction, but different magnitude. Their goal is the same: make our software development and release process faster and more robust.
+ The key difference between the three is in the scope of automation applied. What gets people who are new to the field confused is that they are not mutually exclusive, but include each other, like Russian dolls.
+ Most developers start with Continuous Integration (CI), which is about everyone merging code changes to a central repository multiple times a day. Each merge triggers an automated build and testing sequence for the given project.Depending on the programming language, the program may first need to be compiled. Today there is also an increasing need to package the code in a Docker container. Automated tests then verify specific units of code, UI behavior, application performance, API reliability, and more. Together, all these steps are commonly referred to as the “Build” stage.CI acts as a safety net that lets developers prevent many issues before they reach users. As a result, developers ship code with more confidence, but not necessarily faster — the deployment process may still be manual, long, and error-prone. The best initial investment developers can make is to ensure that their automated test suite is comprehensive and stable enough that they feel safe to deploy every passed CI build to a staging, and later production environment, without a long manual QA (quality assurance) process.

+ Continuous integration involves a series of steps that are automatically performed to integrate code from multiple sources, create a build and test. Each time a build or a set of code passes the tests, it’s automatically deployed out to a staging environment where further testing such as load testing and manual exploratory testing is conducted. This process can be repeated for days depending upon the project delivery requirements.

+ Wikipedia describes Continuous Integration (CI) as “the practice of merging all developer working copies to a shared mainline several times a day.” The CI Model takes Agile a step further by automating the integration and Testing.

+ The thought of integrating new code with the mainline of the application code several times a day can be a scary thought for those more familiar with the waterfall methodology. At a glance, it seems that this would be massively problematic, resulting in the introduction of numerous bugs into the mainline code. However, as the majority of development teams have already discovered, the result is quite the opposite. The code segments being worked on at any given time are much smaller and are therefore easier to both code and debug if there is an issue. So, unlike the waterfall methodology where you create an entire version of the application and then submit it for testing, with continuous integration, the developer submits only small segments of the application at a time. Each of these code segments is then saved and automatically sent to the build server either immediately, or at regular intervals throughout the day. The build is then automatically passed to a test server that executes a series of automated unit tests to ensure that the new code segments work as planned. For additional information on the CI framework, Gartner has published a great article called, “A Guidance Framework for Continuous Integration: The Continuous Delivery ‘Heartbeat,” by Bill Holz and Sean Kenefick.By doing this, the new code segments are built, integrated and tested in mere minutes, providing the developer with immediate feedback on the status of the code and any related issues.

+ Key Strengths of Continuous Integration (CI) Testing
It’s no secret that testing the same test scripts every day can be a highly monotonous duty. Most development teams have found that the automation of test scripts wherever possible goes a long way. Not to mention, it also provides immediate feedback to the developer in mere minutes.
    - __Issue Resolution__ When the automated test scripts do find an issue in the code, because the code  segments are small, the developers have been able to make quick work of issue identification and resolution.
    - __Phased Changeover__ With small iterative changes, studies have confirmed that the migration from an old version of the software to a newer version is much easier because the users are eased into the changes, instead of having to learn a new version of the software all at once.
    - __Improved Team Morale__: Surprisingly, submitting these iterative changes has also improved dev team morale, especially when tasked on larger projects. The reason is that it’s part of our human nature that we like to see accomplishments regularly. Unlike the waterfall methodology, where a large project can drag on for weeks or even months without completing any key milestones, the iterative approach allows developers to achieve multiple milestones per day. This also provides the immediate gratification of seeing their code passing the automated tests several times a day.
    - __Increased Velocity__: Teams have found that with the iterative changes to the code, automated builds, automated testing, and the rapid identification of issues, the overall velocity of the project delivery is significantly faster in comparison to waterfall methodology.
    - __Improved Quality__:
    Because issues are found and resolved with each sprint, those larger, more comprehensive development issues are substantially mitigated. This is because once a sprint has been deployed, subsequent code iterations are then added to the code that has already been proven to be functionally correct. This eliminates the issue of needing to fix multiple incorrectly developed modules because of a coding issue in a single module.
    - __Improved Budget__:
    With the increase in delivery velocity and shifting the identification and resolution of coding issues left, teams are saving a lot of time and resources, which all add up to a healthier bottom line.

**Continuous Deployment (CD)**
---

+ In continuous deployment, every change goes through an automated pipeline and a working version of the application is automatically pushed to production. It does not involve any release approval cycle and the project teams need to ensure that every time a code is updated, tested and released, it works smoothly at the customer’s end. Naturally, a lot depends on the quality of the test suite. With continuous deployment, teams can have multiple software deployments on any given day and don’t have to sweat about a major release

+ Continuous Deployment is a step up from Continuous Delivery in which every change in the source code is deployed to production automatically, without explicit approval from a developer. A developer’s job typically ends at reviewing a pull request from a teammate and merging it to the master branch. A CI/CD service takes over from there by running all tests and deploying the code to production, while keeping the team informed about outcome of every important event.

+ Continuous deployment takes a further step from continuous delivery. It is a software engineering practice that ensures code changes are continuously released into the production environment. The goal is to release a new version whenever developers make changes and automatically get those changes to the end users. 

+ Continuous deployment is the ultimate goal of software development companies. Your company’s development and IT teams must properly prepare to tackle implementing continuous deployment. Production-ready environments and appropriate practices must be put in place to make sure the live environment is up to par. 

+ In continuous deployment, codes are run and maintained in a simulated environment, ensuring that the ultimate quality is taken into consideration. Real-time monitoring of the live environment is also a requirement to keep track of any arising issues and resolve them quickly. 

+ The key benefits of this are similar to those of CDE. However, there are also others that should be mentioned.

    - __Morphed Migration__
    The product gets built iteratively in production and more or less morphs from one version to the next. This approach substantially reduces the anxiety that customers have when they are given a whole new version of the software that they now have to learn.
    Enhanced Delivery Velocity
    Gone are the days of creating code and lobbing it over the fence to builders, who then bounce it to the testers and so on. With continuous deployment, the developer can check code and get a pass/fail notification within minutes. If an issue is detected, they can resolve it and have the new version submitted and into production within a few minutes. If no issues are detected, the new code is moved automatically into production.
    - __Shift Left__
    When a developer checks in code, the automated processes take the code and move it through the entire lifecycle and if it passes each gate, it gets deployed directly to production. This provides the developer with nearly immediate feedback regarding if a code segment has a defect or not. If an issue is detected in the automated tests, the developer is notified and can resolve the issue immediately.
    - __Expedited Tests__
    Testing has traditionally been a bottleneck in the development lifecycle. However, with CD, automated tests can be set up throughout the value stream to be as thorough as needed. This means the testing can be set up at the appropriate stages to address the progression of the code throughout the lifecycle. This can include automated unit tests, integration tests, regression tests, performance tests, and so forth. These can be set up and executed at their respective stations in the lifecycle providing a thorough testing framework to ensure quality. However, because the gate management and handoff from one state to the next are also fully automated, the progression of the code through the lifecycle occurs at light speed when compared to the legacy waterfall approach.
    - __Real World Experimentation__
    This model also allows for real-world experimentation, such as A/B testing, and allows for immediate consumer feedback. For example, if you need to change the location of a certain feature on a website, but you’re not sure of the best new location, you could make the change, monitor real-time customer usage, and make adjustments accordingly.

**Continuous Delivery (CDE)**
+ Continuous delivery helps you build a refined version of the software by continuously implementing fixes and feedback until finally, you decide to push it out to production. In other words, continuous delivery involves human decision-making around what to release to the customers, and when. This forms the basis of the difference between the two.

+ Continuous delivery provides a competitive advantage for organizations that need their deployment decisions to be supported by authoritative human intelligence. It allows teams to deliver new features as they are ready, test working prototypes with real customers and build and evolve more stable, resilient systems.This, in turn, reduces the ongoing costs of evolving products and services, improve their quality and reduce team burnout.

+ There are some exceptions where the concepts of delivery and deployment aren’t as relevant as they are elsewhere; for instance, if you’ve contributed to a library or created an artifact, you are unlikely to deploy it on a running system. In other words, there is no deployment phase. You simply push your code into a repository for other applications to consume. Similarly, with most web apps, teams often don’t have separate build and deploy phases, which means there’s no apparent distinction between the delivery and deployment phase.

+ Being Agile
Working in an Agile environment, you constantly learn from small pieces of work and thereby are able to make improvements before actual deployment.

    - Planning for short cycles, such as 2-week Sprints, allows you to have a smaller bit to review and improve. By incorporating feedback loops along the way you are given important information that illuminates what works and what doesn't work in order to make corrections quickly. Being agile means you can have the infrastructure keep up with changes and match the application development cadence in order to avoid deploying on the "wrong" infrastructure.

    - An Agile environment requires automating the testing phase so it happens fast and provides accurate feedback and can keep up with a Continuous Delivery pace. An agile response comes into play for issues that are reported through the help desk and other user input channels.

+ Continuous Delivery
    - When you are striving for Continuous Delivery, where you can deploy any version at any time on any platform, it forces you to optimize the development process.

    - It's a given that there is 10-30% technical debt on each Sprint. Technical debt includes such things as introducing defects or bugs and releasing a feature on infrastructure that hasn't been developed yet. It's difficult to be perfect. So, just realize that technical debt will occur and look for the feedback loops to give you the information necessary for corrections.

    - Be sure that you get detailed feedback about how the test run went and how the process went at the end of the delivery cycle. These are some examples of questions you can answer in order to improve the process:

    - Did you finish what you thought you would finish?
    - Did you estimate properly?
    - Did it take the same amount of time you thought it would take?
    - Were the tasks done the actual tasks the team had to complete during Sprint execution?
    - Were there a lot of tasks that had to be done that were not planned?
    - In looking at Continuous Delivery, the preferred goal is to be ready and able to deploy 10 or more times per day. If you hit that goal, then deployment can be done every 45 minutes.

    - Continuous Deployment
    Continuous Deployment is actually deploying; however, it doesn't mean you must deploy to production or to the customer every time. For example, you can deploy to QA or to a deployment slot. A deployment slot is an A/B deployment method that allows you to get valuable information without inconveniencing users in the event that a defect leaks through a gap in the testing process. This takes some of the fear and anxiety out of the deployment.

    - One way of deploying to a slot might be to offer an "opt-in" choice for the customer to get an updated version, providing you with a smaller group of users that can serve as a "beta." You always give these users the ability to go back to the former version if they want to do so.

    - Continuous Improvement
    Engaging in Continuous Improvement is an important part of Continuous Delivery and Continuous Deployment. Continuous Improvement requires that you amplify feedback loops by:

    - Setting baselines. Be sure you have a starting point from which you can measure.
    Monitoring important metrics. The key metric is deployment frequency of 10 or more times per day. There are some other side effect metrics like mean time to recover, mean time to change, and defect to new work ratio, but these aren't as important as the deployment frequency.
    Identifying bottlenecks. Feedback loops during Sprints give you information on any congestion or blockages in the cycle.
    Every time you find a gap in the process you have an opportunity to do a "gap fill" with a new test, new script, or new process. Create tests that test for defects. Set acceptance criteria based on input from the users. And, automate Acceptance Testing so that testing gets run on every commit to the source code.