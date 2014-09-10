####Grails Cucumber Example
##Step Definitions

	Given(~'^an Invader named "([^"]*)"$') { String name ->
		//persist quote
	}

	When(~'^a Quote is requested for "([^"]*)"$') { String name ->
		to QuotePage
	}

	Then(~'^we see "([^"]*)"$') { String quote ->
	    def invasionQuote = page.fetchInvasionQuote()
	    assert invasionQuote == quote
	}

<p class="fragment roll-in">`test/cucumber/steps/quote_steps.groovy`</p>
<p class="fragment roll-in"><em>Gorm no longer supported!</em></p>
<p class="fragment roll-in"><em>Use <a href="https://github.com/alkemist/grails-remote-control/">Remote Control Plugin</a> instead!</em></p>
<p class="fragment roll-in"><em>Use Geb!</em></p>
