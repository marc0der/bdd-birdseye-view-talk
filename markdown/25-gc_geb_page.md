####Grails Cucumber Example
##Geb Page

	class CandidatePage extends Page {
	    static url = "candidate/list"
	    static at = { title ==~ /Candidate List/ }

	    static content = {
	        candidateList { $("div.list table", 0) }
	        candidate { candidateName -> 
	        	module CandidateModule, $("#$candidateName")
	        }
	    }

	    def isCandidateInList(String candidateName){
	        def candidateRow = candidate(candidateName)
	        return candidateRow ? true : false
	    }
	}

`test/functional/page/CandidatePage.groovy`