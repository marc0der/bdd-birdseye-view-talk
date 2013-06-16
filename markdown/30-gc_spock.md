####Grails Cucumber Example
##Spock Specification

	@TestFor(CandidateController)
	@Build([Candidate])
	class CandidateControllerSpec extends Specification {

		void "should return a list of available candidates"(){
			given:
			def grails =  new Candidate(name:'grails',defaultVersion:'2.2.2').save()
			def groovy =  new Candidate(name:'groovy',defaultVersion:'2.1.5').save()

			when:
			def result = controller.list()

			then:
			result.candidateInstanceList.contains grails
			result.candidateInstanceList.contains groovy
		}
	}
