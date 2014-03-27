####Grails Cucumber Example
##Geb Module

class QuotePage extends Page {

    static url
    static at = { title == "Invader Zim Quotes" }

    static content = {
        quote { $("#message") }
    }

    def fetchInvasionQuote(){
        quote.text()
    }
}

`test/functional/modules/QuotePage.groovy`
