####Grails Cucumber Example
##Configuration

	cucumber {
		tags = ["~@manual"]
		features = ["test/cucumber"]
		strict = true
		glue = ["test/cucumber/steps", "test/cucumber/support"]
	}

<p class="fragment roll-in">`grails-app/conf/CucumberConfig.groovy`</p>

<p class="fragment roll-in"><em>Replaces Test Runner <a href="/cuke-talk/#/5/3">configuration</a>.</em></p>