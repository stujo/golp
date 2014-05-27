Golp! Search, Find and Share Your Favorite Things!

---

#Rails Track - Overview

Welcome to your new job at Golp! we are a startup and you are on the team

This week we are going to build an application together!

* Each day we will share our User Stories with you

* Each User Store will describe one feature

* Your job will be to implement the feature assigned to you

* We will share a master repository and you will fork it, just like the open source

    * Many of you will work on the same feature each day

    * You will each work in your own repo

    * You must submit a working solution to the feature assigned to you

    * Each day we'll pick one implementation of each feature and integrate it into master

    * We will then sync up the repositories with the master and begin the process again

* Some features will be core MVP features which all team members must complete

* Some additional features will be available to team members who have completed the day's MVP

You will independently with limited instructor support, you are expected to research and find your own solutions to
the feature challenges. This is the time to build your confidence that you can solve problems without assistance


#Pre-Work

Before we can use this workflow we'll need to set up the git repositories

* This is our master repository:
  * [https://github.com/wdi-sf-march-2014/golp](https://github.com/wdi-sf-march-2014/golp)
* Fork this repository to your GitHub account
* Clone your fork locally


#Daily Feature Workflow

* Instructors Present User Story to the team:

    * User Story
      * Has Name
      * Has Persona
      * Has Description
      * Has Feature Test(s)

* Instructors then present overview of relevant material and  provide you with some pointers and documentation
references

* ~15 Minutes: Group discussion to ensure shared understanding of feature

* 5 Minutes: break

* ~15 Minutes : SOLO investigation (no coding)

* ~15 Minutes : Pair Discussion (no coding)

* ~15 Minutes Group discussion of possible solution directions, clarification of approach

* SOLO work on the feature (see below)

* At the end of the allotted time Every Student will explain their code to one other student

* Then switch roles with partner

* Then Instructors will pick one student explain their partner's code


#SOLO work
On this project you are working independently and on this project you are NEVER working on master repo directly

Before you start working on a feature:

* Ensure local git repository is up to date and synced with master repo
* Ensure you are on master branch
* Ensure git status is clear
* Create a new feature branch from the updated master branch
    ```(master)$ git checkout -b feature_name```
* Make your changes on this branch

Once you've completed your feature work:

* Commit and push your branch to your github repo:
    ```(feature_name)$ git push origin feature_name```
* On github create a Pull Request from your feature_name branch to the master repo's feature_name branch
* Review your pull request with another student to get feedback
* Make any changes you both feel are necessary and make sure all tests are passing

Once you feel your feature is ready for prime time:

* Work with an instructor on a review of your pull request
* You may need to make more changes or 'sync' your fork with the master repo before your branch can be merged
instructions on syncing are provided below, don't worry, your instructor will walk through this with
you (if it's necessary)


