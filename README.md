# I_Cloud_SpecFlow_GitHubActionsExample
A Spec flow BDD UI test project example with GitHub Actions and reporting

Feature: Add Elements
! As a user I should be able to add elements on the page. Max number of elements can be added is N.
	a. navigate to The Internet (https://the-internet.herokuapp.com/add_remove_elements/)
	b. add n number of elements
	c. assert that n number of elements exist on the page

Background: Navigate to the page
	When I navigate to the herokuapp add elements page

Scenario: Add N specified number of elements on the page
	Given I am on the add-remove elements page
	When I click on the add element button <N> times
	Then I should see <N> elements on the page
Examples: 
	| N  |
	| 0  |
	| 1  |
	| 12 |
	| 99 |
