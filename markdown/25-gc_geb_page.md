####Grails Cucumber Example
##Geb Page

	class QuotePage extends Page {

		static url = "/zim-grails/invader"
		static at = { title == "Invader Zim Quotes" }

		static content = {
		    quote { $("#message") }
		}

		def fetchInvasionQuote(){
		    quote.text()
		}

	}

`test/functional/page/QuotePage.groovy`
