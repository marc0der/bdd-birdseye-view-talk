####Grails Cucumber Example
##Controllers

#####Controller

	class InvaderController {
		def index(String id) {
		    [quote: Quote.findByName(id)]
		}
	}

#####URL Mapping

	"/invader/$name"(controller: "invader")