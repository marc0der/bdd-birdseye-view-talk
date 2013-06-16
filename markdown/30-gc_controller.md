####Grails Cucumber Example
##Controller

#####Controller

	class CandidateController {
	    def list(Integer max) {
	        params.max = Math.min(max ?: 10, 100)
	        [candidateInstanceList: Candidate.list(params), 
	        	candidateInstanceTotal: Candidate.count()]
	    }
	}