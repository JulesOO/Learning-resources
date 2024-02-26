- [Way of working](#way-of-working)
  - [Collaboration](#collaboration)
  - [Agile](#agile)
  - [Platform/product teams](#platformproduct-teams)
- [DevOps](#devops)
  - [Continuous Integration](#continuous-integration)
  - [Continuous Delivery](#continuous-delivery)
- [Developer culture](#developer-culture)
  - [Culture](#culture)
  - [Talent](#talent)
- [Enterprise IT](#enterprise-it)
  - [IT transformations](#it-transformations)
  - [Architecture](#architecture)
  - [Metrics](#metrics)
  - [Operations](#operations)
- [Other](#other)
  - [Security](#security)
  - [Cloud](#cloud)
  - [Hardware](#hardware)

## Way of working

### Collaboration
* [What does larger scale software development look like?](https://www.youtube.com/watch?v=Dl-BdxNRUqs): Best-practice large scale software development. why are there multiple environments (dev,test,prod), how do teams collaborate with each other and with the client
* [What is the "best way" to develop software applications?](https://www.youtube.com/watch?v=oNmcX6Gozg0): “gold standard” software development process (only works for small teams)
* [Things I Learnt The Hard Way (in 30 Years of Software Development)](https://blog.juliobiason.net/thoughts/things-i-learnt-the-hard-way/): Practical collection of stuff under the umbrella "keep it simple".
* [Software development topics I've changed my mind on after 6 years in the industry](https://chriskiehl.com/article/thoughts-after-6-years): Another great list of tips.
* [Google Engineering Practices Documentation](https://google.github.io/eng-practices/): Great guide that explains how to do proper code reviews
* [On Navigating a Large Codebase](https://blog.royalsloth.eu/posts/on-navigating-a-large-codebase/): Great set of practical tips on how to deal with large, messy code bases
* [Why the world needs a software bill of material now](https://drrispens.medium.com/why-the-world-needs-a-software-bill-of-materials-now-5a565df65dff): Good summary of rationale for emerging domain of software bill of material and how it can not only reduce risk but also save cost.
* [In depth research and trends analyzed from 50+ different concepts as code](https://www.jedi.be/blog/2022/02/23/trends-and-inventory-of-50-as-code-concepts/) Overview of everything as-code from Patrick Debois
* [GitLab's Guide to All-Remote](https://about.gitlab.com/company/culture/all-remote/guide/): Great guide from the Gitlab experts on remote working

### Agile

* [Why Scrum is the Wrong way to build software](https://medium.com/@ard_adam/why-scrum-is-the-wrong-way-to-build-software-99d8994409e5): Critique on SCRUM methodology from engineer's perspective  (why it does not empower engineers to work on the right things). Valid arguments but the author does not offer a solution. There is probably something to be said on differentiating the approach/degree of process you put in place based on the strengths of engineers you have in your team.
* [Reality Driven development](https://www.brightball.com/articles/reality-driven-development-fixing-project-management-in-software): Long explanation to make the excellent point that Kanban + very limited use of pair programming is the way to go.
* [5 ways to tune your standup](https://techbeacon.com/5-ways-tune-your-standup): Practical tips to make your standup actually useful
* [You don't need a standup](https://medium.com/@jsonpify/you-dont-need-standup-9a74782517c1): Alternative view on Agile ceremonies that shows that there is more than one way of doing Agile. Reminds me of the C4 method of the late Pieter Hintjens.
* [Embracing asynchronous communication](https://about.gitlab.com/company/culture/all-remote/asynchronous): Great deep-dive from Gitlab on how to move maximally to asynchronous communication
* [Engineering team management](https://github.com/kdeldycke/awesome-engineering-team-management#readme): Great collection of links on the topic
* [I’ve been employed in tech for years, but I’ve almost never worked](https://emaggiori.com/employed-in-tech-for-years-but-almost-never-worked/): The reason to focus on the real reason for doing Agile: The customers
* [Why backlogs are harmful, why they never shrink, and what to do instead](https://lucasfcosta.com/2023/02/07/backlogs-are-useless.html): Excellent article on backlog management

### Platform/product teams

* [Free-market software development](http://matt.chadburn.co.uk/notes/teams-as-services.html) and [Tips for-inhouse teams in a free market software culture](https://medium.com/ft-product-technology/tips-for-in-house-teams-in-a-free-market-software-culture-d18ba80c8c4): Concrete case study of how the Financial Times' teams dealing with internal software/tooling operate. Great set of concrete tips ranging from mission statement of such teams, how they interacte with their consumers, culture, documentation, ...
* [https://techbeacon.com/app-dev-testing/forget-monoliths-vs-microservices-cognitive-load-what-matters](https://techbeacon.com/app-dev-testing/forget-monoliths-vs-microservices-cognitive-load-what-matters): Great description on how to think about architecture and team organization and the different patterns to apply / signals to watch out for.
* [Product for Internal Platforms](https://medium.com/@skamille/product-for-internal-platforms-9205c3a08142): Fantastic article that explains how to think about product management in platform teams. First one that I've seen and it does an excellent job at it.
* [Who should write Terraform?](https://zwischenzugs.com/2022/08/08/who-should-write-the-terraform/): Excellent post that describes trade-offs involved in setting up central platform teams

## DevOps

### Continuous Integration

* [Why I love Trunk Based Development](https://medium.com/@mattia.battiston/why-i-love-trunk-based-development-641fcf0b94a0): Strong argumentation in favor of trunk-based development. See also [Trunk Based Development](https://trunkbaseddevelopment.com/)
* * [Please stop recommending Git Flow!](https://georgestocker.com/2020/03/04/please-stop-recommending-git-flow/): Or why trunk-based development is the way to go and git flow makes things too complex (note that git flow is originally developed  for products with multiple version in production, for example software installed on customer premise).
* [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/): Simple and easy to follow specification for commits that allows to generate release notes automatically.
* [Why you should not use feature branches](https://fire.ci/blog/why-you-should-not-use-feature-branches/): Love the last quote in the article ``A good common ground is to use short lived branches that last 1 or 2 days max and merge them to the main branch. This way you can human control what gets in and still integrate code fast.``. This is probably the best approach for most teams.
* [Patterns for Managing Source Code Branches](https://martinfowler.com/articles/branching-patterns.html): Nothing new but great description of different branching strategies and their trade-offs. 

### Continuous Delivery

* [Keep database deploys separate](http://www.philandstuff.com/2018/04/04/keep-database-deploys-separate.html): database changes should follow all the good practices of continuous delivery (e.g., source controlled) but they should not be done together with code changes.
* [Terraform for Teams](https://www.runatlantis.io/): cool tool that integrates infrastructure changes in a clean way in your github/gitlab/bitbucket workflow
* [5 Lessons Learned From Writing Over 300,000 Lines of Infrastructure Code](https://blog.gruntwork.io/5-lessons-learned-from-writing-over-300-000-lines-of-infrastructure-code-36ba7fadeac1): Practical approach to write infrastruture-as-code in a maintainable and scalable way
* [7 Pipeline Design Patterns for Continuous Delivery](https://www.singlestoneconsulting.com/blog/7-pipeline-design-patterns-for-continuous-delivery/): Good overview of elements of continuous delivery pipeline
* [Production Oriented Development](https://paulosman.me/2019/12/30/production-oriented-development.html): Fantastic summary of how to think about development practices. Couldn't agree more.
* [Testing microservices, the sane way](https://medium.com/@copyconstruct/testing-microservices-the-sane-way-9bb31d158c16): Lengthy explanation of testing practices, trade-offs to make when to use which tests and the "step up rule" 
* [Testing in production, the safe way](https://medium.com/@copyconstruct/testing-in-production-the-safe-way-18ca102d0ef1): Excellent overview of techniques to do quality engineering on production systems and how it makes your dev, test environments simpler and in some cases not needed anymore.
* [State of Mutation Testing at Google](https://ai.google/research/pubs/pub46584): Cool approach to test the effictiveness of a test suite and detect parts of the code that are not covered probably by tests. Also interesting how Google integrates this in the code review process.
* [Lean Testing or Why Unit Tests are Worse than You Think](https://blog.usejournal.com/lean-testing-or-why-unit-tests-are-worse-than-you-think-b6500139a009): Provides a balanced view on which tests to invest in when. In particular advocates for much less reliance on unit tests except for a few specific cases such as testing algorithms and reusable libraries.
* [21 Types of Software Testing Every Engineer Should Be Using for Better Results](https://stratoflow.com/types-of-software-testing/): Good structured overview of the different types of testing

## Developer culture

### Culture
* [Compare countries](https://hofstede-insights.com/product/compare-countries/): Compares cultural differences between countries on the 6-D model.
* [Five Things I did to Change a Team's culture](https://zwischenzugs.com/2018/02/24/5-things-i-did-to-change-a-teams-culture/): Super-practical case study that shows how cultural change requires concrete and tangible actions that are not "artificial" for the team.
* [The Trouble With Promises: Patrick Debois Explains Serverless And 'Service-Full' Culture](forbes.com/sites/oracle/2017/10/12/the-trouble-with-promises-patrick-debois-explains-serverless-and-service-full-culture/): Inspiring talk from the founder of the DevOps movement where he argues for service-full architectures and the need to apply the culture and devops practices outwards as we move to a world where applications are basically a composition of externally consumable services.
* [How to hire](https://hbr.org/2018/01/how-to-hire): Excellent description from Netflix's former HR manager on hiring practices and the importance of HR to work together with business.
* [How to Deal with Difficult People on Software Projects](https://people.neilon.software/): Fantastic overview of different archetype of people in a software project and how to deal with them. 
* [Google Says the Best Bosses in the World Do These 10 Things](https://www.inc.com/justin-bariso/google-says-best-bosses-in-world-do-these-10-things.html): Great overview of 10 things to look out for in your managers and team leads
* [The Anatomy of a Dev Team](https://www.rookout.com/blog/the-anatomy-of-a-dev-team): Which one do you recognize?

### Talent
* [Programmer Moneyball: Challenging the Myth of Individual Programmer Productivity](https://insights.sei.cmu.edu/sei_blog/2020/01/programmer-moneyball-challenging-the-myth-of-individual-programmer-productivity.html): Great article that questions the 10x programmer myth and instead argues that differences are mostly due to "worse" performers and individual variations.
* [It's Differentiation Season (Redux)](https://www.alancolquitt.com/single-post/2019/01/21/its-differentiation-season-redux): Don't do individual variable pay!
* [The Platform Engineer](https://engineering.razorpay.com/the-platform-engineer-db2b21434911): Amazing article on what it takes to be a real platform engineer!
* [Dropbox Engineering Career Framework](https://dropbox.github.io/dbx-career-framework/overview.html): Dropbox's framework for evaluation of various engineering profiles
* [How to mentor software engineers](https://xdg.me/mentor-engineers/): Good framing of different types of mentoring and how to tackle.
* [CTO day 7: Lucky Lotto, chaos engineering but for teams](https://danlebrero.com/2021/06/30/cto-dairy-lucky-lotto-chaos-engineering-for-teams/): Amazing concept for building resilient teams using a simple and positive technique while at the same time freeing time up for continuous improvement
* [Your CTO Should Actually Be Technical](https://blog.southparkcommons.com/your-cto-should-actually-be-technical/): 5 good reasons why your CTO should be technical
* [How to drive away your best engineers](https://blog.hulacorn.com/2021/09/08/how-to-drive-away-your-best-engineers/): Quite to the point :-)
* [37 Years Ago, Steve Jobs Said the Best Managers Never Actually Want to Be Managers. Science Says He Was Right](https://www.inc.com/jeff-haden/37-years-ago-steve-jobs-said-best-managers-never-want-to-be-a-manager-science-says-he-was-right.html): "If your boss could do your job, you're more likely to be happy at work."

## Enterprise IT

### IT transformations
* [In praise of SWARMing](https://dannorth.net/2018/01/26/in-praise-of-swarming/): Excellent overview on what it takes to really transform an organization. This posts makes some excellent points on the usefullness (or lack thereof) of frameworks (DAD, SAFE, LESS and the likes), the role leadership needs to play, the need to change how money is allocated early on in the transformation and how to do change management (communication, education, influencing). SWARMing = Scaling Without A Religious Methodology :-)
* [The Cost Center Trap](http://www.leanessays.com/2017/11/the-cost-center-trap.html): Incredible rich and spot-on article that makes the point that the fundamental focus on cost in most IT organizations is destructive for operating as a truly digital company and how capitalization of software leads to large (and often failing) IT projects. Or how a conversation with the CFO is key for letting any digital or Agile transformation succeed.
* [Agile Transformation at Ericsson](https://www.infoq.com/articles/agile-transformation-ericsson): Excellent write-up on success factors in Agile transformations: start with leadership, quality of coaches is important, train-the-trainer model, importance of storytelling and symbolic changes and an excellent point on the need for somebody to keep long-term perspective.
* [Yes, You Can Eliminate Bureaucracy](https://hbr.org/2018/11/the-end-of-bureaucracy): Excellent case study on transformation of a traditional company to an ecosystem of startups. In concept very similar to an enterprise agile model but pushes thinking much further and frames everything in terms of the customer.
* [Scaling engineering organizations](https://stripe.com/atlas/guides/scaling-eng): Excellent guide to key HR processes within Stripe. Stresses the point of not wanting to go too fast.
* [Gitlab](https://about.gitlab.com/company/strategy/): Gitlab company strategy. Particulary interested are their [OKRs](https://about.gitlab.com/company/okrs/) and [KPIs](https://about.gitlab.com/handbook/business-ops/data-team/metrics/), both of which can serve as an inspiration for Agile Infrastructure providers.

### Architecture
* [How do we scale web applications?](https://www.youtube.com/watch?v=NeWMO_vFpe8): How are web applications scaled (e.g. horizontal/vertical scaling, load balancers, CDNs) and when should you use each scaling solution
* [How to improve a legacy codebase](https://jacquesmattheij.com/improving-a-legacy-codebase/): Excellent and practical article on how to take an unmaintained codebase and get it back into shape (as an alternative to a big system replacement that will most likelly fail)
* [You're not actually building microservices](https://www.simplethread.com/youre-not-actually-building-microservices/): Argument in favor of monoliths and indications on why you're microservices architecture is actually behaving like a monolith (or worse)
* [The death of microservices madness in 2018](https://www.dwmkerr.com/the-death-of-microservice-madness-in-2018/): Balanced arguments on when to use microservices and the fact that it is more an implementation pattern than an architectural pattern, which implies that good architecture design is still needed!
* [App migration checklist](https://cloud.google.com/blog/products/storage-data-transfer/app-migration-checklist-how-to-decide-what-to-move-to-cloud-first): Good checklist/stuff to consider when migrating applications to cloud.
* [Choose Boring Technology](https://mcfunley.com/choose-boring-technology): This post becomes relevant every year. I love the visualization of good technology choices when you take operational burden into account.
* [Amazon EventBridge: The biggest thing since AWS Lambda itself](https://www.trek10.com/blog/amazon-eventbridge/): Amazon EventBridge might indeed prove to be a fantastic innovation since it allows Lambda functions and other applications to integrate nicely in a federated event-based system. This would require a standardized way of publishing the format (and versioning of that format) of events and describing when events are emitted.
* [API Gateways are going through an identity crisis](https://medium.com/solo-io/api-gateways-are-going-through-an-identity-crisis-d1d833a313d7): Great taxonomy of API-related functionality (service mesh, reverse proxy, API gateways
* [Exit the haunted forest](https://increment.com/software-architecture/exit-the-haunted-forest/): Great and practical ways to recognize and deal with unmaintainable code bases
* [Using Kubernetes to rethink your system architecture and ease technical debt](https://stackoverflow.blog/2021/05/19/rethinking-system-architecture-can-kubernetes-help-to-solve-rewrite-anxiety/): Cool description on how to think incrementally about system modernization
* [Hunting Tech Debt via Org Charts](https://bellmar.medium.com/hunting-tech-debt-via-org-charts-92df0b253145): Great perspective on how org and architecture are linked to each other
* [Real-world migration challenges](https://newsletter.pragmaticengineer.com/p/real-world-engineering-challenges: Great set of practical examples of migrations
* [You Want Modules, Not Microservices](http://blogs.newardassociates.com/blog/2023/you-want-modules-not-microservices.html): Excellent arguments on why you shouldn't just go with the microservices hype but focus on good old architecture principles
* [Stop saying technical debt](https://stackoverflow.blog/2023/02/27/stop-saying-technical-debt/): How to change the conversation around technical debt
* [Things I Wished More Developers Knew About Databases](https://medium.com/@rakyll/things-i-wished-more-developers-knew-about-databases-2d0178464f78): Great list

### Metrics
* [Building for the 99% Developers](https://future.com/software-development-building-for-99-developers/): Great overview of some of the pitfalls of chasing the big tech companies when it comes to how they develop software.
* [Internal Development Platform](https://internaldeveloperplatform.org/): Overview page of emerging field
* [The Gruntwork Production Framework](https://docs.gruntwork.io/guides/production-framework/): Great overview of tech architecture to cover
* [Engineering Effectiveness Handbook](https://www.okayhq.com/handbook/): Tips and metrics
* [How to be a -10x Engineer](https://taylor.town/-10x): Funny article with anti-patterns
* [Four Magic Numbers for Measuring Software Delivery](https://medium.com/onzo-tech/four-magic-numbers-for-measuring-software-delivery-55b1dd01eca): Practical guide on how to operationalize measuring and visualizing the 4 key metrics from the Accelerate DevOps book.
* [Selecting the Right User Metric](https://medium.com/sequoia-capital/selecting-the-right-user-metric-de95015aa38): Structured and practical way of determining which usage metric to track for your product.
* [System Dashboard Design](http://onemogin.com/observability/dashboards/practitioners-guide-to-system-dashboard-design.html): Four part article on practicalities of system dashboard design and how to make them as self-explanatory and useful as possible.
* [Everyone Thinks They’re Managing by Outcomes. Here’s How to Actually Do it](https://www.producttalk.org/2019/10/managing-outcomes/): Managing on outcomes ... easier said than done :-)
* [Fast and flexible observability with canonical log lines](https://stripe.com/gb/blog/canonical-log-lines): Description of how Stripe does logging with canonical log lines as a nice addition to structured logging.
* [The SPACE of Developer Productivity](https://queue.acm.org/detail.cfm?id=3454124): No really new information but a nice article on ho wto think about developer productivity as a balanced set of metrics.
* [Engineering productivity can be measured](https://www.okayhq.com/blog/engineering-productivity-can-be-measured): Great view on how to think about engineering productivity as blockers at the team level.
* [Metric Display Standards](https://medium.com/salesforce-ux/metric-display-standards-54736533c81): Structured methodology for metrics dashboard design
* [Metrics-driven product development is hard](https://blog.doubleloop.app/metrics-driven-product-development-is-hard/): Great way to think about hierarchy of metrics
* [Delivery Lead Time in Practice](https://isthisit.nz/posts/2022/delivery-lead-time-in-practice/): Good deep-dive on how to use delivery lead time metric (from code commit to production)

### Operations
* [On designing and deploying internet-scale services](http://mvdirona.com/jrh/talksAndPapers/JamesRH_Lisa.pdf): Iconic paper from the LISA conference that details a lot of the SRE/DevOps practices and mindsets before they were formally documented. Contains some great insights that go against current thinking (e.g., minimize dependencies to the ones that are really worth it vs micro-services thinking). [This](https://blog.acolyer.org/2016/09/12/on-designing-and-deploying-internet-scale-services/) contains a more recent commentary and a link to an up-to-date checklist that can be used. 
* [Serverless Ops: What to do when the server goes away](https://serverlessops.io/blog/serverless-ops-what-do-we-do-when-the-server-goes-away): Overview of tasks/responsibilities of an operations engineer on a team operating a Serverless Infrastructure. Provides a good overview of the tasks/skills needed to operate Serverless infrastructure, not sure I agree with the positioning of operations engineer on the team.
* [An example escalation policy — CRE life lessons](https://cloudplatform.googleblog.com/2018/01/an-example-escalation-policy-CRE-life-lessons.html) and [Applying the Escalation Policy — CRE life lessons](https://cloudplatform.googleblog.com/2018/02/applying-the-escalation-policy-CRE-life-lessons.html): Practical example on how to balance velocity and reliability using error budgets
* [Know thy enemy: how to prioritize and communicate risks - CRE life lessons](https://cloudplatform.googleblog.com/2017/05/know-thy-enemy-how-to-prioritize-and-communicate-risks-CRE-life-lessons.html): Systematic method on quantifying and prioritizing operational risks
* [Why should your app get SRE support? - CRE life lessons](https://cloudplatform.googleblog.com/2017/06/why-should-your-app-get-SRE-support-CRE-life-lessons.html): Great overview on how to size SRE teams, think about the number of parallel services they can support and for which services to consider SRE support and for which not
* [Defining SLOs for services with dependencies - CRE life lessons](https://cloudplatform.googleblog.com/2018/05/Defining-SLOs-for-services-with-dependencies-CRE-life-lessons.html): Excellent and practical overview on how to deal with dependencies that impact your SLO's
* [Best Practices for Setting SLOs and SLIs For Modern, Complex Systems](https://blog.newrelic.com/engineering/best-practices-for-setting-slos-and-slis-for-modern-complex-systems/): Excellent and practical article on how to think about SLI's and SLO's for a system as a whole and individual capabilities (backend, data, ui)
* [Operability questions](https://github.com/ConfluxDigital/operability-questions/blob/master/operability-questions.md) and [Run book template](https://github.com/SkeltonThatcher/run-book-template/blob/master/run-book-template.md) are great checklists to understand operations requirements early in the dev cycle.
* [Toil](https://landing.google.com/sre/sre-book/chapters/eliminating-toil/) Even outside of the context of SRE teams, measuring toil is important. It is one of the three main categories of work: engineering work ("new stuff"), toil ("stuff that can be eliminated") and overhead (e.g., meetings). Measuring toil can provide a fact-based discussion on the value of e.g., investing in test or deployment automation.
* [SLO Workshop](https://www.usenix.org/sites/default/files/conference/protected-files/srecon18emea_slides_fong-jones.pdf): Excellent and practical intro to different types of SLI/SLO's and how to define them.
* [(A few) Ops Lessons We All Learn The Hard Way](https://www.netmeister.org/blog/ops-lessons.html): Great and funny list that shows (sometimes trivial) copmlexity of dealing with operations
* [Writing Runbook Documentation When You’re An SRE](https://www.transposit.com/blog/2020.01.30-writing-runbook-documentation-when-youre-an-sre/): Great and practical description with links to templates on how to write runbooks.
* [Observability and the Misleading Promise of AIOps](https://thenewstack.io/observability-and-the-misleading-promise-of-aiops): Couldn't have written it in a more clear manner. AIOps is bs.
* [Presentation: Findings From The Field](https://www.adaptivecapacitylabs.com/blog/2020/07/16/presentation-findings-from-the-field/): Great insights on incident handling practices for managers and practicioners
* [How to successfully Hand Over Systems ](https://developers.soundcloud.com/blog/how-to-successfully-hand-over-systems): Practical checklist on how to hand over systems.
* [The Art of Logging](https://betterprogramming.pub/creating-a-human-and-machine-freindly-logging-format-bb6d4bb01dca): Practical guide with best practice fields that should be used for consistent logging

## Other

### Security
* [Everything you should know about certificates and PKI but are too afraid to ask](https://smallstep.com/blog/everything-pki.html): Excellent and in-depth overview of everything you need to know about using or setting up your own PKI.
* [How to get started with Threat Modeling, before you get hacked.](https://hackernoon.com/how-to-get-started-with-threat-modeling-before-you-get-hacked-1bf0ea3310df): Practical intro to threat modeling with the whole team.
* [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org/): Detailed cheat sheets for various security topics.
* [ScoutSuite](https://github.com/nccgroup/ScoutSuite): Great tool to audit your cloud platform for potential security violations
* [A Guide to Threat Modelling for Developers](https://martinfowler.com/articles/agile-threat-modelling.html): Great and practical way to get started and sustain threat modelling as a core practice in Agile product teams.
* [On Establishing a cloud security program](https://www.marcolancini.it/2021/blog-cloud-security-roadmap/): Comprehensive and actionable overview

### Cloud
* [Cloud Naming Convention](https://stepan.wtf/cloud-naming-convention/): Describes importance and practical approach to establish cloud naming conventions
  
### Hardware
* [CPU 101](https://cpu.land/): Deep-dive guide on how CPUs work
* [Nand2Tetris](https://www.nand2tetris.org/): University course on building a computer starting from logic gates. Build a CPU, RAM, Operating system, Compiler and Virtual Machine.