##Cucumber Anatomy

###Test Runner

	import cucumber.api.CucumberOptions
	import cucumber.api.junit.Cucumber
	import org.junit.runner.RunWith

	@RunWith(Cucumber)
	@CucumberOptions(
	    format=["pretty", "html:build/reports/cucumber"],
		strict=true,
	    features=["features"],
	    glue=["src/test/steps"]
	)
	public class RunCukesTest { }

<p style="color:grey" class="fragment roll-in">`src/test/groovy/RunCukeTests.groovy`</p>
