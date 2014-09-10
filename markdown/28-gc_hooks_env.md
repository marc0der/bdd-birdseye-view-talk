####Grails Cucumber Example
##Environment Hooks

	import geb.binding.BindingUpdater
	import geb.Browser

	import static cucumber.api.groovy.Hooks.After
	import static cucumber.api.groovy.Hooks.Before

	System.setProperty("geb.build.baseUrl", "http://localhost:8080")

	Before () {
	    bindingUpdater = new BindingUpdater (binding, new Browser ())
	    bindingUpdater.initialize ()
	}

	After () {
	    bindingUpdater.remove ()
	}

<p class="fragment roll-in">`test/cucumber/support/env.groovy`</p>

<ul>
	<li class="fragment roll-in"><em>Use for any long running fixture</em></li>
	<li class="fragment roll-in"><em>Hooks run before and after each scenario</em></li>
	<li class="fragment roll-in"><em>Like @BeforeClass and @AfterClass in JUnit</em></li>
</ul>