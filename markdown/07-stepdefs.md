##Cucumber Anatomy

###Step Definitions

	import static cucumber.api.groovy.EN.*

	Given(~'^the input "([^"]*)"$') { String input ->
		//some groovy code
	}

	When(~'^the calculator is run$') { ->
		//some groovy code
	}

	Then(~'^the output should be "([^"]*)"$') { String output ->
		//some groovy code
	}

<p style="color:grey" class="fragment roll-in">`src/test/cucumber/steps/add_steps.groovy`</p>
