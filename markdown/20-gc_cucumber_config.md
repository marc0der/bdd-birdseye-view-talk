####Grails Cucumber Example
##Configuration

	cucumber {
		tags = ["~@wip"]
		features = ["test/cucumber"]
		glue = ["test/steps", "test/support"]
		formats = [ "html:target/test-reports/cucumber" ]
	}

<p class="fragment roll-in">`grails-app/conf/CucumberConfig.groovy`</p>

<p class="fragment roll-in"><em>Replaces Test Runner <a href="/cuke-groovy-talk/#/4/3">configuration</a>.</em></p>
