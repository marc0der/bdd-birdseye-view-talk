####Grails Cucumber Example
##Step Definitions

	Given(~'^the candidate "([^"]*)" exists with default version "([^"]*)"$'){ String name, String defaultVersion ->
	    def candidate = new Candidate(
	    	name: name, 
	    	defaultVersion: defaultVersion
	    )
	    assert candidate.save()
	}
	When(~'^I visit the Candidate page$') { ->
	    to CandidatePage
	    at CandidatePage
	}
	Then(~'^I see "([^"]*)" listed$') { String candidateName ->
	    assert page.isCandidateInList(candidateName)
	}

<p class="fragment roll-in">`test/cucumber/steps/manage_candidates.groovy`</p>
<p class="fragment roll-in"><em>Gorm!</em></p>
<p class="fragment roll-in"><em>Geb!</em></p>
