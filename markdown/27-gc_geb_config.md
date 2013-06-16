####Grails Cucumber Example
##Geb Configuration

	import org.openqa.selenium.chrome.ChromeDriver

	driver = {
	    new ChromeDriver()
	}

`test/functional/GebConfig.groovy`

<ul>
	<li class="fragment roll-in">
		<em>Remember to <a href="https://code.google.com/p/chromedriver/downloads/list" target="#">download</a> chromedriver!</em>
	</li>
	<li class="fragment roll-in"><em>Place it in root of project folder.</em></li>
	<li class="fragment roll-in"><em>...or use any selenium driver you like.</em></li>
</ul>