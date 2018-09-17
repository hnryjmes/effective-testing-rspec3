## Effective Testing with RSpec 3
###### by Myron Marston and Ian Dees

#### Notes

Introduction

* 'effective' - tests that are more valuable than the time spent to write them

* Behavior-Driven Development

Chapter 1 - Getting Started With RSpec

* How to install RSpec and write your first spec / How to organize your specifications using describe and it / How to verify desired outcomes with expect / How to interpret test failures / How to keep your specs free of repeated setup code

* Effectiveness. Do the benefits of writing the test outweigh the costs?

* First spec: groups, examples, expectations

* "A test validates that a bit of code is working properly."

* "A spec describes the desired behavior of a bit of code."

* "An example shows how a particular API is intended to be used."

* Arrange, Act, Assert

* hooks: common setup code

* "Our recommendation is to use these code-sharing techniques where they improve maintainability, lessen noise, and increase clarity."

* Exercise 1. "We've shown you three primary ways to reduce duplication in RSpec: hooks, helper methods, and let declarations. Which way did you like best for this example? Why? Can you think of situations where the others might be a better option?" - hook and let methods are quite similar, helper methods are pretty intuitive. it would depend on the context for the test which to use. overuse of the before syntax could be risky and/or harder to maintain compared to let, which is more narrowly specified.

Chapter 2 - From Writing Specs to Running Them

* How to generate readable documentation from your specs / How to identify the slowest examples in a suite / How to run just the specs you care about at any given moment / How to mark work in progress and come back to it later

* testing all: a row of green dots, and red Fs

* "By choosing a different formatter, you can tailor the output to your needs."

* Example group, examples, nesting, footnote numbers

* Syntax highlighting with CodeRay, identifying slow examples, running what you need i.e. searching by keyword

* Run the most recent failing spec, the --only-failures flag

* focus: add 'f' to method name (e.g. context becomes fcontext) [use temporarily!]

* understanding tag filtering and passing metadata to rspec

* pending examples - tracking your work in progress

* Exercise 2. The --next-failure flag is different from the --only-failures flag in that it only returns the first failure and then stops further tests. Once the failure has been addressed, the next failure becomes something else.

* using the shell you can make rspec output to html or to json!

Chapter 3 - The RSpec Way

* How your specs can give your confidence in your code / How a good test suite makes refactoring possible / How to guide your design using your specs with behavior-driven development (BDD)

* "Specs increase confidence in your project."

* Make change easy for yourself

* "By surfacing the pain of a design problem early, specs allow you to fix it while it's cheap and easy to do so."

* Making development more like a game...

* Important point: making tests run quickly means you're more likely to test

* don't overtest...

* three types of specs: acceptance, unit, integration

Chapter 4 - Starting On the Outside: Acceptance Specs

* expenses app in Ruby + Sinatra + Sequel + SQLite

* (why Sinatra and not Rails? for simplicity and learning how to test...)

* Setting up the app: what do we want to test first?

* using HTTP: GET and POST requests

* workflow: update the spec, then update the app

Chapter 5 - Testing in Isolation: Unit Specs

* The difference between acceptance specs and unit specs / How to use dependency injection to write flexible, testable code / The use of test doubles/mock objects to stand in for real ones / How to refactor your specs to keep them clean and readable

* using dependency injections

* "A test double is an object that stands in for another one during a test."

* waiting to refactor code

* "It's tempting to start factoring out duplicate code while you're still writing your specs. Avoid that temptation: get your specs passing first, and then refactor. That way, you can use your specs to check your refactoring."

* 
