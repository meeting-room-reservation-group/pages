---
layout: page
title: About
permalink: /about/
---

In this group we develop together a small application _Meeting Room Reservation (System)_. The idea is to show many steps, from gathering _Business Requirements_, setting up the project, doing _Test Driven Development_, adding the project to GitHub, etc, etc, till _Deployment_. All done in blog posts, so everyone should be able start, and follow these steps.

But it can also be used, to lookup how certain things are done, like using _Cucumber Features_, or _Continuous Integration_ by [Travis-CI](https://travis-ci.org/) in a complete (mini) project.


## Project Overview


### Business Requirements

The business requirements should be explained in the form of [Specification by Example](https://en.wikipedia.org/wiki/Specification_by_example) use-cases. These _use-cases_ will be written in the [Cucumber](https://cucumber.io/) - [Gherkin](https://cucumber.io/docs/reference) format. The idea is that everyone should be able to read those _feature_ files. Each feature exists of one or more _scenarios_. Each _scenario_ contains at least one concrete example, of some requirement.


### Architecture

All the services will be created in the [Resource Oriented Architecture](https://en.wikipedia.org/wiki/Resource-oriented_architecture)(ROA) style.


## Frameworks / Libraries

__General__

- [Jersey](https://jersey.java.net/)

__Testing__

- [Cucumber](https://cucumber.io/)  
  WikiPedia [Cucumber](https://en.wikipedia.org/wiki/Cucumber_(software))  
  [Gherkin](https://cucumber.io/docs/reference)


## Tools

- Source Code Management  
  [git](https://git-scm.com/)
- Source Code Sharing  
  [GitHub](https://github.com/)
- Build Tool  
  [Maven](https://maven.apache.org/)
- Continuous Integration (CI) / Continuous Delivery (CD) / Continuous Deployment (CD)  
  [Travis-CI](https://travis-ci.org/)
- Code Editor  
  [Eclipse](http://www.eclipse.org/)  
  __INFO__ Eclipse is _not_ required, but several details will be explained by using Eclipse as the code editor.
