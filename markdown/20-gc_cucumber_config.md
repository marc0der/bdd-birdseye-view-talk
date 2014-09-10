####Grails Cucumber Example
##Configuration

	cucumber {
	    tags = ["~@wip"]
	    features = ["test/cucumber"]
	    glue = ["test/steps"]
	    formats = [ "html:target/test-reports/cucumber" ]
	    strict = true
	}

<p class="fragment roll-in">`grails-app/conf/CucumberConfig.groovy`</p>

<p class="fragment roll-in"><em>Replaces Test Runner <a href="/cucumber/#/4/3">configuration</a>.</em></p>
