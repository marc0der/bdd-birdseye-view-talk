####Grails Cucumber Example
##Hooks: Clean up GORM

	After () {

	    def sessionFactory = applicationContext.getBean("sessionFactory")
	    sessionFactory.currentSession.flush()

	    def dataSource = applicationContext.getBean("dataSource")

	    //clean fixtures
	    println "Deleting the fixture..."
	    def db = new Sql(dataSource)
	    db.execute("DELETE FROM CANDIDATE;")

	    sessionFactory.currentSession.clear()
	}

<p class="fragment roll-in">`test/cucumber/support/fixture.groovy`</p>

<ul>
	<li class="fragment roll-in"><em>GORM's Hibernate session leaks across Scenarios.</em></li>
	<li class="fragment roll-in"><em>Feels sleezy :-P</em></li>
</ul>
