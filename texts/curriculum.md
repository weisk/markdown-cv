# Francesc Mallafre Lopez

## Key Technologies & Frameworks

- Javascript, from the inside out, since the early days to the latest specs / apis.
- Typescript, for type sharing, compile-time errors, and all the goodies
- React, from early versions up to the latest v18 specs.
- CSS, in full depth, and many of its dialects: sass, less,...
- HTML, also in full depth, and many of its dialects: pug/jade, jsx, tsx...
- React libraries: UI Components, state managers, routing frameworks,
- React internal APIs: Context, Providers, Suspense/Fallback,
- Nodejs, also extensively used. To define APIs, services, or just any kind of application.
- Git: as the holy grail of code management. Git Flow, as methodology.
- Could providers, network architecture and security protocols. AWS, GCP, azure, DO...
- GraphQL, Apollo server.
- MongoDB, Redis, ... (noSQL databases, document oriented)
- PosgreSQL, mysql, and more generally Relational Databases.
- CI/CD, using many tools from jenkins to travis, until most recently github actions and workflows.
- Testing: Jest, react testing library, cypress for e2e testing, pact.js for integration testing.
- Bundlers & Pipelines, from Webpack v5, esbuild. Federated modules, monorepos with Lerna, and Turbo.
- Containerised environments with Docker, compose.
- Architecture management with Kubernetes.

## Extract

Computing and programming enthusiast with a passion for algorithms, programming, and everything related to technology. Having an engineering background, I always had the drive to understand the underlying mechanisms in computing, which always amazed me. To this day I still wonder at the complexity of mechanisms in internet, and how it's even possible that everything works!

The web and specifically FrontEnd area is my strongest skill, and also my most professionally developed area. I have extensive knowledge of all aspects of web applications, from UI/UX design to backend development, APIs, data management, networking/performance optimization, CI/CD pipelines, and cloud infrastructure.

Professionally I have worked in many companies, each one of them being like a different universe. but I also developed all by myself projects which span the whole spectrum, as a software architect. With that I mean devising all the pieces that will form a whole structure, to solve each particular problem..

From the requirements definition, to drafting an entity relationship model. Designing the Data structures, and deciding if it would make sense to make it relational, non-relational, graph based. Defining API contracts, in order for the different components to collaborate. Designing cloud architectures: what kind of servers are needed, and what capacity are they going to support. Would it require servers, or could it be served from a CDN. Would it require scalability, thus then load balancing policies, and virtual net infrastructure. Using the major providers, that is AWS, Google cloud platform, Azure, Firebase, Digitalocean.


## WORK EXPERIENCE

### Adevinta : Senior Frontend Engineer, Jul 2021 - November 2023

I've worked in Adevinta as a frontend engineer, mainly to modernize and maintain the Web UI used to configure content moderation within all marketplaces of Adevinta. To provide some more context, the main business in Adevinta is basically online marketplaces, for buying/selling used items. Think of ebay as an example.

You can imagine how huge is the volume of generated user content, and thus how essential is to minimise the amount of spam or illegal content that gets published. For this, adevinta has a series of machine learning modules, each one performing a particular task, that work together in order to determine if one piece of content is spam or not. That prediction comes in the form of a score, a percentage, that allows the users of the platform - fraud analysts, to choose the threshold at which the content can be 'automatically' moderated, and thus the rest will fall to manual moderation.

And then the challenge is unifying all these tools in a single process, intuitive, that abstracts away all the details and allows for non-tech savvy users to understand what's going on, and even to more advanced users to tweak those parameters. All this is implemented in a web application, which has been my main focus of work in adevinta.

One of my biggest and most challenging projects I've faced is this: to migrate an old architecture of a series of micro apps, in different repositories, into a monorepo that contains everything within. From shared libraries, like the UI components, common libraries for certain functionalities, and the different modules that comprise each route.

There is one main React app wrapper, the Shell, that does all the necessary imports and defines the routes, and then all the different modules: shared components, libs, and modules. All this is bundled in chunks, that are loaded on demand, using dynamic imports, depending on the route loaded.

It is all coded through the latest React APIs (up to v18), using a unified type system with typescript, and bundled with Webpack module federation.

The CI/CD is implemented in different layers, of testing (react testing library, cypress, sonar), peer-reviewing (enforced through github PR policies), and deployment to different stages (using github actions workflows).

Another big project I handled during my time here was, refactoring all 3rd party api calls into a main single API implemented with GraphQL, and the Apollo framework. This in itself is a huge different topic that deserves another full document, but to not extend myself too much, I will just outline the main points of it:

  - Defines an API for all XHR calls the frontend needs,
  - Unifies all of them in the same graphql server,
  - going through the same security checks on every request, like, Authentication, and Authorisation,
  - shares the Data Types with the frontend monorepo, in Typescript,
  - Integrates the external calls made to all 'real backend' machine-learning modules, which are mostly Python services.


### marketScape : Software Engineer Sep 2019 - Dec 2020

This is a saas used for gathering and collecting data, in order to gain intelligence, reporting and visibility of various topics. This service was actually used by High level agencies, or government organisms, not open to end users, since it dealt mainly with fraud / illegal activities data acquisition and recognaissance. But to give an overview, the data analysed would be things like: fashion market trends, consumption of alcohol, music reproductions, drug consumption, religious fanatism, cross-referenced with social media activities.

My role here is was implementing the frontend, and designing the architecture for new features. A big chunk of my work was porting an outdated server-side rendered architecture to a more modular, interactive webapp. Using angular since that was a client requirement.

I also work on abstracting inefficient legacy implementations into micro-services oriented API, that could come in NodeJS simple apps, to stateless Lambda functions.

### Kasaz.com : Senior Frontend Developer Feb 2019 - Aug 2019

Joined this little startup that aims at the real estate sector in Barcelona.

My task was mainly to refactor the public facing products, in order to increase the sites 'crawlability' by search engines, and also to make a pleasant User Experience that loaded fast, and looked beautifully.

Conversion from a server-side rendering server to a bundled Multi-Page application, keeping the main business logic on a small package. It was important here to keep many parts of the site pre-rendered, since the SEO ranks were essential for the bussiness. We implemented a combo of SSR + hydration once loaded into a browser.

As mentioned, there was also a big emphasis on maintaining and improving SEO scores across different engines. That involved a lot of studying the particular quirks of each provider, but mainly Google, and keeping track of what google considers good / bad: avoid hidden content, work on genuine content, avoid duplication of links, define good site maps, use proper semantic HTML, render responsive sites that work on any screen size, etc.

### Haufe-Umantis AG Swiss : Senior Frontend Developer Oct 2017 - Nov 2018

Working as a frontend developer expert in technologies such as React (+Redux,Router,..) and Angular(1,2,4).

### Propertyfinder : Senior Frontend Developer Feb 2016 - Mar 2017

Propertyfinder is a leading real estate company in Dubai.

I was hired as a Javascript developer, in a team of 4 people including me. My role was initially to work closely with the team lead to study their current infrastructure to find potential bottlenecks and improve the whole stack with a more modern philosophy.

This was accomplished on 4 main levels:

1.- Refactored an old PHP server-side rendered codebase towards a dynamic - client side rendered with Javascript and React,

2.- Migrating a huge monolith architecture into single resposibility microservices. One example is the implementation of a microservice that dealt with everything related to image operations: resizing, conversion, edition, formatting, watermarking, etc.

3.- Implement testing for the frontend, on two levels: unit-testing for dumb function behaviour, using mocha and chai for assertions, and end-to-end testing for browser expectations; using JSDom to render pages.

4.- Automate the frontend code building process: Using gulp to gather all dependencies, concatenate all the javascript files, compile Sass to css, render html templates, etc.

I also led a small team of 3 frontend developers on a side project, which could be written from scratch and allowed for experimentation. Made entirely on React+Redux, with Jest+Enzyme for component/e2e testing.


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

### Roche Diagnostics S.L.: Front End Technology Programmer (Jul 2011 - Jan 2013)

Working on a Laboratory Information System (LIS) for hospitals and healthcare professionals. Here started my journey in the professional programming world, and the first time I learned about Javascript.

Full migration from a .NET client/server architecture, to web-based architecture, fully HTML5/CSS3
compliant. Design of screens , tables, gadgets , graphics , charts , etc.. for the application , mainly using the combination of HTML5/CSS3 & javascript, SVG .


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
