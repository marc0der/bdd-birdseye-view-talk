####Grails Cucumber Example
##Gherkin Feature

	Feature: Invader Quotes

	  Scenario: Invader GIR quotes by Name
		Given an Invader named "GIR"
		And the Invader "GIR" says "Can I be a mongoose dog?"
		When a Quote is requested for "GIR"
		Then we are taken to the Quote Page
		And we see "Can I be a mongoose dog?"

<p class="fragment roll-in">`test/cucumber/quote.feature`</p>
