##Cucumber Anatomy

###Test Runner

	import cucumber.api.junit.Cucumber
	import org.junit.runner.RunWith

	@RunWith(Cucumber)
	@Cucumber.Options(
		format=["pretty", "html:build/reports/cucumber"],
		strict=true,
		features=["src/test/cucumber"],
		glue=["src/test/cucumber/steps", "src/test/cucumber/support"],
		tags=["~@manual", "~@review"]
	)
	public class RunCukesTest {
		//leave me empty!
	}

<p style="color:grey" class="fragment roll-in">`src/test/groovy/RunCukeTests.groovy`</p>
