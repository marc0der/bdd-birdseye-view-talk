####Grails Cucumber Example
##Controller

#####Controller

	class InvaderController {
		def index(String id) {
		    [quote: Quote.findByName(id)]
		}
	}
