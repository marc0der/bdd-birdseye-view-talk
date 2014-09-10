####Grails Cucumber Example
##Configuration

	dependencies {
		...
		test "org.codehaus.geb:geb-junit4:0.7.2" 
		test "org.seleniumhq.selenium:selenium-chrome-driver:2.32.0" 
		test "org.seleniumhq.selenium:selenium-support:2.32.0" 
		...
	}

	plugins {
		...
		test ':cucumber:1.0.1'
		compile ':remote-control:1.5'
		...
	}

<p class="fragment roll-in">`grails-app/conf/BuildConfig.groovy`</p>
