####Grails Cucumber Example
##Step Definitions

	Given(~'^an Invader named "([^"]*)"$') { String name ->
		quote = new Quote(name:name)
	}

	When(~'^a Quote is requested for "([^"]*)"$') { String name ->
		to QuotePage
	}

	Then(~'^we see "([^"]*)"$') { String quote ->
	    def invasionQuote = page.fetchInvasionQuote()
	    assert invasionQuote == quote
	}

<p class="fragment roll-in">`test/cucumber/steps/quote_steps.groovy`</p>
<p class="fragment roll-in"><em>Gorm!</em></p>
<p class="fragment roll-in"><em>Geb!</em></p>
