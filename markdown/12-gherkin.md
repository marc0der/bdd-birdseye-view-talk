##Cucumber Anatomy

###Gherkin

	Feature: Adding
		
		Scenario: Add two numbers
			Given the input "2+2"
			When the calculator is run
			Then the output should be "4"

<p style="color:grey" class="fragment roll-in">`src/test/cucumber/adding.feature`</p>