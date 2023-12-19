# Francesc Mallafre Lopez

## Key Technologies & Frameworks

- Javascript, from the inside out, since the early days to the latest specs / apis.
- Typescript,
- React, from early versions up to the latest v18 specs.
- CSS, in full depth, and many of its dialects: sass, less,...
- HTML, also in full depth, and many of its dialects: pug/jade, jsx, tsx...
- React libraries: UI Components, state managers, routing frameworks,
- React internal APIs: Context, Providers, Suspense/Fallback,
- Nodejs, also extensively used. To define APIs, services, or just any kind of application.
- Git: as the holy grail of code management. Git Flow, as methodology.
- GraphQL, Apollo server.
- MongoDB, Redis, ... (noSQL databases, document oriented)
- PosgreSQL, mysql, and more generally Relational Databases.
- CI/CD, using many tools from jenkins to travis, until most recently github actions and workflows.
- Testing: Jest, react testing library, cypress for e2e testing, pact.js for integration testing.
- Bundlers & Pipelines, from Webpack v5, esbuild. Federated modules, monorepos with Lerna, and Turbo.
- Containerised environments with Docker, compose.
- Architecture management with Kubernetes.

## Extract

Computing and programming passionate, my favourite distraction that is algorithms and programming has been my professional career.

The web and specifically FrontEnd area is my strongest skill, and also my most professionally developed area. I have extensive knowledge on all the aspects related to web applications, from the ui to the backend, api's, data, networking / performance, ci/cd, infrastructure, and the main cloud providers.

From my engineering background, I always had the drive to understand the underlying mechanisms in computing, which were also my funniest hobbies to practise.

Professionally I have worked in many companies, each one of them being like a different universe. but I also developed all by myself projects which span the whole spectrum, as a software architect. With that I mean devising all the pieces that will form a whole structure, to solve a customer's particular needs.

From the requirements definition, to drafting an entity relationship model. Discussing what storage technologies would be adequate, relational, non-relational, graph based. Defining a Restful API contract, implementing it using any technology.
Designing a user interface aiming at the best possible user experience, adapted to the technology needs: desktop, mobile.
Defining the whole architecture on the cloud: what servers are needed, and what capacity are they going to support. It could be that a frontend is served from an edge CDN, while the backend is isolated from the internet and the public access point is a load balancer to distribute the load. AWS, Google cloud platform, Azure, Firebase, Digitalocean. They all do basically the same thing, but normally the choice depends on the requirements of the customer. (They may already have a contract with Microsoft, or with Google Apps...).


## WORK EXPERIENCE

### Adevinta : Senior Frontend Engineer, Jul 2021 - November 2023

I have been working for 2+ years in Adevinta as a frontend engineer. My main occupations and duties have been to develop and modernize the UIs of the company, in particular the platforms used internally across all departments of Adevinta. To further explain, there are many departments within Adevinta, but all of them orbit around the same segment: online 2nd hand Marketplaces. Think of ebay, as an example. There are many different markets / brands on many countries, but all of them use the same internal tooling for the biggest problem they all have in common: the fight against spam or fraudulent content.

So, in our department we developed and maintained the tools that all marketplaces use in order to moderate content, before being published to the world. To do this, there are a series of machine learning modules, that analyze the content from different perspectives, and assign a score or probability that that content is not legitimate. From analyzing the text content, to find forbidden patterns like URLs, emails, etc., through processing the images, to a drag&drop rule engine that allows the moderators to define complex heuristics to mark content as spam or not.

The main target of my team was to maximise the amount of content that gets automatically moderated. There are some configurable ratios that allow you to define which percentage of probability can be automatically processed, and which percentage is not clear enough so that it goes to a manual moderation.

Well, all this platform is streamline and offered in a web interface that allows you to tweak each module, and that has been my main focus.

One of my biggest and most challenging projects I've faced is this: to migrate an old architecture of a series of micro apps, in different repositories, into a monorepo that contains everything within. From shared libraries, like the UI components, common libraries for certain functionalities, and the different modules that comprise each route.

There is one main React app wrapper, the Shell, that does all the necessary imports and defines the routes, and then all the different modules: shared components, libs, and modules. There is a main bundle that contains the shell, and the minimum required components to render the app, and then all the modules are lazy-loaded on demand through dynamic imports.

It is all coded through the latest standards and specs, sharing all the same type definitions, and the versioning is done with lerna/nx per package.

All testing is also handled through the same monorepo, using react testing library and cypress, and all handled through github actions workflows.

Another big project I handled during my time here was, refactoring all 3rd party api calls into a main single API implemented with GraphQL, and the Apollo framework. This in itself is a huge different topic that deserves another full document, but to not extend myself too much, I will just outline the main points of it:

  - Defines an API for all XHR calls the frontend needs,
  - Unifies all of them in the same graphql server,
  - going through the same security checks on every request, like, Authentication, and Authorisation,
  - shares the Data Types with the frontend monorepo, in Typescript,
  - Integrates the external calls made to all 'real backend' machine-learning modules, which are mostly Python services.


### marketScape.com : Software Engineer Sep 2019 - Present

Crawling the internet, in order to collect data about specific topics from different sources. Normalize, analysis and synthesis of this data, in order to find and group differentiative elements from that topic. A topic can be anything: fashion market trends, consumption of alcohol, music reproductions, drug consumption, religious fanatism.
Sources can be anything that feeds data from the public, social networks, polls, reports.
So depending on every use case, the election of sources and topics can deliver the following:
- Gain advantadge over the competence by reacting fast.
- Iterate on the data, decide business strategy based on it.
- Detect criminal groups, isolate hot spots of activity, find bad people.

My role here is not only frontend but also architect of the different parts of the software. My main expertise and where I focused more is on the frontend layer, using angular8 , make a less monolithic structure.
However I also helped to migrate towards a micro-services-oriented API , contributed on better ways to store and fetch the data, how to design the algorithmics for the web spiders, as well as dev-ops tasks like making the develop - test - deploy cycle simpler and faster.

### Kasaz.com : Senior Frontend Developer Feb 2019 - Aug 2019

Joined this little startup that aims at the real estate sector in Barcelona, bringing fresh and innovative ideas.
My task has been to boost the front part of the site's visibility and quality, using my acquired skills over the
years. So after some study, I designed a plan.
Conversion from a server-side rendering server to a compiled SPA on React. Well not exactly single, because
it has some static sections, so actually a Multi-Page application, keeping the main business logic on a small
package. SEO-wise, we don't want to break current search engines ranks, so we have to keep server side
rendering. So implement a system that renders on the server, with a piece of code that "hydrates" the static
site, converting it to an SPA, only if the client supports javascript.
Work together with a designer to create a branding. Re-design the structure of the page to make it more
intuitive, easier to use. Keep it simple: cut a lot of unnecessary content or sections, or move it somewhere
else, so that users don't look cluttered, and it doesn't cause distractions.
SEO: Try to follow all the standards and guides provided by search engines. Eliminate all penalising things, or
things that make the search engine think you are cheating, like for example, hidden texts, duplicate url's, etc..

### Haufe-Umantis AG Swiss : Senior Frontend Developer Oct 2017 - Nov 2018

Working as a frontend developer expert in technologies such as React (+Redux,Router,..) and Angular(1,2,4).

### Propertyfinder : Senior Frontend Developer Feb 2016 - Mar 2017

Propertyfinder is a leading real estate company in Dubai. The company specializes in putting in touch sellersThis resume is made with CVwizard.com.
with buyers, through a web platform. It's free for clients to register on the website, however ad publishers
have to pay a monthly subscription to be able to post their ads. There are different subscription tiers, from
the simple ones, to the premium ones, which also allow you to access in-depth analytics of client behaviour
and user tracking.
I was hired as a Javascript developer, in a team of 4 people including me. My role was initially to work
closely with the team lead to study their current infrastructure to find potential bottlenecks and improve the
whole stack with a more modern philosophy. This was accomplished on 4 main levels:
1.- Refactored an old PHP server-side rendered codebase towards a dynamic - client side rendered with
Javascript.
2.- Proposed a migration from monolithic architecture to a micro-service oriented structure; trying to isolate
components with isolate responsibilities from the other parts. For example, we implemented a new image
treatment micro-service which allowed for on-demand resizing, conversion, and overall image
manipulation.
3.- Implement testing for the frontend, on two levels: unit-testing for dumb function behaviour, using mocha
and chai for assertions, and end-to-end testing for browser expectations; using JSDom to render pages.
4.- Automate the frontend code building process: Using gulp to gather all dependencies, concatenate all
the javascript files, compile Sass to css, render html templates, etc.
On another side I also worked in a company's side project made entirely with React+Redux, with Jest+
Enzyme for component/end-to-end testing. On this part I proposed to move the codebase from ES5 to a
more modern ES6 based code
My role was initially to assess the status and get a feel for the whole stack, reporting to a team lead, but
after 2 months the team lead was promoted to CTO and I, in turn, to the frontend team lead. I had to
manage the 3 developers work, we used Pivotal as a time tracker / task organiser. We did daily SCRUM
meetings and weekly reports of team performance.





### Cloud Digital: Front End Lead Developer Mar 2014 - Jan 2015

In charge of the development of the front-end of a media distribution platform. Built on top of Angular.JS,
Bootstrap for the layout and Google Material for design components. Using Coffeescript to produce quality
Javascript code. Bower for dependency management. Grunt for wiring assets and libraries, building and
cleaning the code, and delivering deployable artifacts. Several Javascript libraries to leverage specific
functionalities, like Lodash (former Underscore.js) , Jquery, Moment.js, Growl, Flow.js, ngTagsInput ...
Built the marketing site at http://www.cloud.xxx
Using Git & Github for version control. JIRA as a sprint planner & task reporting. Confluence as a team wiki.
Also built the staging & production systems on Amazon Web Services. VPC as the infrastructure, OpsWorks
for resource provisioning & code deploying, Route53 for domain management, S3 as the storage layer... AndThis resume is made with CVwizard.com.
CloudFlare in front of everything to speed up transfers.
Integrated a error tracking & logging system based on Sentry using its javascript client Raven.js. We
managed to log all javascript errors to an interface knowing all the debug info: error culprit, logged user,
referrer URL, server response, along with the javascript stack trace.

### Scytl: Javascript Developer Aug 2013 - Jan 2014

Worked as a FrontEnd Javascript developer, using mainly Angular.js , jQuery , underscore and more libraries.
Hired for a 4 month project, which was an online electronic voting system for the country of Ecuador. I was
given the opportunity to continue but I had to decline due to my studies in computer engineering, which
had to be finished in that time. I can give the full explanation for this if requested.
Advanced Javascript programming: prototypal inheritance, asynchronous execution, design patterns such
as private/privileged/public members, first-class citizen functions ...Implemented javascript logic for
controllers,views and models, with all the benefits Angular.js has to offer: two-way data binding, custom
directives for extended HTML, live page updates, back-end communitaction ... etc

### Roche Diagnostics S.L.: Front End Technology Programmer (Jul 2011 - Jan 2013)

Working on a Laboratory Information System (LIS) for hospitals, intended to manage everything that
happens on a hospital. From patients and the tests they have to take, the tubes and samples each test
takes, doctor scheduling, all work places, interfacing with the diagnostic equipment and the hospital
computer systems..
Full migration from a .NET client/server architecture, to web-based architecture, fully HTML5/CSS3
compliant.
Design of screens , tables, gadgets , graphics , charts , etc.. for the application , mainly using the
combination of HTML5/CSS3 & javascript, SVG .
On the other side, using InterSystems Caché for the back-end, a database management system from
InterSystems that provides object and SQL access to the databases.
The project management was done with IBM ClearQuest for task divisions, using SCRUM metodology
meetings.
As from code source control, using Microsoft's Team Foundation Server and Perforce for windows.


## PROJECTS

I have been fiddling with web technologies since very young, becoming more experienced through the
years and later accepting gigs and contracts with clients. In the projects section you can see a portfolio of products I built, mainly as a freelancer or some of them as a cofounder.

### https://raiseyourwebsite.com
This is a personal project, in collaboration with a designer partner, using cutting edge technologies: It's an
SPA built with React that sits on top an Express.js server, using ES6 compiled with webpack, it's fully
responsive (desktop+tablet+mobile), and it is also a Progressive Web App with a service worker which
allows it to work offline. It does fancy things like server side rendering with async data fetching. TechnologicThis resume is made with CVwizard.com.
key points are: react, react router v4, redux, CSS Modules, ES6 javascript, isomorphic rendering, d3 graph
visualization, mail server, and deployed using PM2 and git.


### https://schoolhouse.io/
Schoolhouse is a healthcare knowledge sharing platform and social network. It is meant for medical
students to get access to quality information, as well as healthcare professionals to keep up with the latest
improvements. It is designed to split the knowledge in all areas of the medicine, from a top-bottom
perspective, and splitted by the different approaches it may have: Medical, Surgical, Biomedical,
Pharmacological, and Physiological. Currently it's on a private beta with Universitat Internacional de
Catalunya (UIC), where it's part of an experiment to score the students using their contributions on the
platform. A more thorough explanation can be done, if requested.
Also, I can provide code and demos.


### http://peer2.cash
This is a platform to allow exchange from crypto currencies to fiat currencies, .e.g.: 1BTC to 400$. The SPA is a
minimalistic panel that displays a trading form which can be used to obtain an offer, and fullfill the
requested information to accept the offer. Coded in AngularJS mainly. There are some algorithms in the
backend to perform crawling of bitcoin markets and crush the data to obtain suitable offers at every
request. More info can be described as per request.
https://stratagems.syngular.es
Prototype landing page for a project that died shortly after its birth. It was meant to be a web-crawler, user
analytics, SEO all around product. With a subscription model type, users could get insights on their preferred
domains, providing valuable data as to increase search engine presence and user visitors.
Several private projects
Worked on internal managing webapps, from ERP and CRM to CMS-type projects. More info available on
request.

## Codes

Things I made, borrowed, want to learn, or just felt the need kept secure.

https://github.com/weisk
https://gist.github.com/weisk
https://gitlab.com/weisk
https://bitbucket.org/franml/
https://jsfiddle.net/user/weisk/fiddles/
https://codepen.io/weisk/
https://codesandbox.io/u/weisk/sandboxes

## EDUCATION

Computer Science September 2007 - July 2014
Universitat Autònoma de Barcelona
"Ingeniería superior en Informática".
This is equivalent to a Bachelor of Science + Master of Science, in a more recent graduation system; it was 450 credits pre-bolgna process.
