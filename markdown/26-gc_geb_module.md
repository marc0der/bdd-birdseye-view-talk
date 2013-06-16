####Grails Cucumber Example
##Geb Module

	class CandidateModule extends Module{
	    static content = {
	        name { $("#name") }
	        defaultVersion { $("#default") }
	    }
	}

`test/functional/modules/CandidatePage.groovy`