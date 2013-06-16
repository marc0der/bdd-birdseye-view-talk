####Grails Cucumber Example
##Gherkin Feature

	Feature: Manage Candidates

	  Scenario: List Candidates
        Given the candidate "Grails" exists with default version "2.2.2"
        And the candidate "Groovy" exists with default version "2.1.4"
        When I visit the Candidate page
        Then I see "Grails" listed
        And I see "Groovy" listed

<p class="fragment roll-in">`test/cucumber/manage_candidates.feature`</p>