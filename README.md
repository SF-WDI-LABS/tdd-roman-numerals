<!-- 
authors: @nathanallen
 -->

# <img src="https://cloud.githubusercontent.com/assets/7833470/10423298/ea833a68-7079-11e5-84f8-0a925ab96893.png" width="60"> TDD Roman Numerals

<img width="400" src="https://media.giphy.com/media/FRu9PpyFEzV7y/giphy.gif">

| Objectives |
| :---- |
|   Configure a project to use RSpec |
|   Explore the methodology of Test Driven Development |
|   Write expectations that test method behavior |
|   Use the Red, Green, Refactor pattern |


In today's lab we will be creating a Converter that takes in a base 10 integer and returns a Roman Numeral string:

| Input | Output |
| :---- | :---- |
| 1 | "I"  |
| 2 | "II" |
| 3 | "III" |
| 4 | "IV" |
| 5 | "V" |
| 6 | "VI" |
| 7 | "VII" |
| 8 | "VIII" |
| 9 | "IX" |
| 10 | "X" |


## Test Driven Development
Test Driven Development can be thought of as a 3 step processs described as "Red, Green, Refactor":

1. Write the test first. Make sure the expectation is failing. ("red")
    * Why? Because if the test passes right away we have a "false positive".
2. Write code to pass the test ("green")
    * It's common to break existing features when you add a new feature. Make sure that _all_ of your tests are passing!
3. Stop and cleanup ("refactor")
    * Is your code DRY? Are your tests DRY? As you make changes, run your tests frequently to ensure your code still works.

> When _pair programming_ one strategy is to play "ping pong". One person writes the test, the other person writes code to pass it. Then you switch roles.

## Setup
Before you can start writing tests, you need to setup the RSpec test suite in your project. Please follow the official [setup instructions](https://relishapp.com/rspec/docs/gettingstarted) to install and configure the `rspec` gem (that means you should have a `Gemfile`!), and setup your first test.

We recommend you save your tests or "specs" in a `/spec` folder because this is the default location `rspec` uses. Since we are testing our `Converter` class which lives in `converter.rb`, we will name our spec file "/spec/converter_spec.rb" to match.

> Make sure you are in the _root_ of your project when you run the `rspec` command!

#### Writing Expectations
You will need to familiarize yourself with the "built-in matchers" included in the dependent `rspec-expectations` library:
* http://www.rubydoc.info/gems/rspec-expectations/frames#Equivalence
* http://www.rubydoc.info/gems/rspec-expectations/frames#Comparisons

## Bonus
Want anther challenge? Try creating a "numbers to words" converter. It should accept an integer and convert it into english words:

| Input | Output |
| :---- | :---- |
| 1 | "one"  |
| 10 | "ten" |
| 21 | "twenty one" |
| 101 | "one hundred and one" |

## Resources

- http://rspec.info/
- https://relishapp.com/rspec/docs/gettingstarted
