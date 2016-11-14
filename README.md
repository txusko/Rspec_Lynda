# Rspec
## Rspec is a testing framework for Ruby

Writing code to test other code

"R" = Ruby
"Spec" = Specification

Spec: An executable example that tests whether a portion of code exhibits the expected behaviour in a controlled context

## What is Rspec?

* Given ome context
* When some event occurs
* Then I expect some outcome
* Given ... When ... Then ...
* Rspec is written is Ruby
* Uses a domain-specific language (DSL)
* Sometimes not very Ruby-like
* Learn Ruby first

## Rails

* Rails is most common use for Rspec
* Rails not required for Rspec
* First basic Ruby with Rspec

## Wht are software tests important?

### Reasons not to test:
- writing tests requires more time
- time is money

### Reasons to test:
- writing tests finds bugs
- simulates critical thinking
- covers edge cases (extremes)
- exposes poorly written code (code smells)
- confidence when refactoring/improving code
- confidence when adding features
- confidence when upgrading related software
- confidence during code deployment
- saves development time!
- saves headache
- helps to sleep at night :)

### Always test?
- small application may not need testing
- testing is more critical as complexity increases
- most developers start testing as they gain experience

## Thinking in User Stories
* Description of the experience of a user of your software
* Excellent planning tool
* Excellent communication tool with developers
* Excellent communication tool with clients
* Describes a single step in the user experience

### User Story #1
* Given that a user is not logged in
* When the user visits the login page
* Then the user should see form fields for username and password and a submit button

### User Story #2
* Given that a user is not logged in and is viewing the login form
* When the user enters a valid name and password and submits the form
* Then the site should redirect them to th approriate user page
(happy path)

### User Story #3
* Given that user is not logged in and is viewing the login form
* When the user enters a valid username and an invalid password and submits the form
* Then the site should return a not valid generic page and return the login page
(unhappy path)

## User Stories
* Defines feature scope and edge cases
* Defines perfectly-sozed portions of code for testing
* No "spaghetti code"
* 1 : 1 ration of story to spec

## Writing good tests
1. What to Test
  * You only have to test the parts that need to work - ha ha
  * How much test coverage we need
  * depends on complexity too
  * existing code: write test by priorities
  * Happy path => users get what they want
  * Unhappy path => when things dont work out and we need to handle it
  * Edge cases
  * Any bug that gets fixed

2. What not to Test
  * Basic Ruby
  * Basic Ruby on Rails
  * Third party APIs
  * Behaviour being tested already

## More advice
- A bad, partial or broken test can be worse than none
- Keep your test suite fast, you will run it more often
- Run tests often
- Every time you do a commit or push code
- Keep your test passing all the time
- Avoid writing brittle test

## Configuration
|Basic settings | new
|--|--|
|--no-color| --color|
--format progress, --format documentation
--no-profile, --profile
--no-fail-fast, --fail-fast
--order defined, --order random
