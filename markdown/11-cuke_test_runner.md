##Cucumber Anatomy

###Test Runner

	import cucumber.api.junit.Cucumber
	import org.junit.runner.RunWith

	@RunWith(Cucumber)
	@Cucumber.Options(
		format=["pretty", "html:build/reports/cucumber"],
		strict=true,
		features=["src/test/cucumber"],
		glue=["src/test/steps"],
		tags=["~@manual", "~@review"]
	)
	public class RunCukesTest { }

<p style="color:grey" class="fragment roll-in">`src/test/groovy/RunCukeTests.groovy`</p>
