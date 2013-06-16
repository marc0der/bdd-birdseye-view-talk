####Grails Cucumber Example
##GSP

	<g:each in="${candidateInstanceList}" 
		status="i" var="candidateInstance">
		<tr>
		<td id="${candidateInstance.name}">
			${fieldValue(bean: candidateInstance, field: "name")}
		</td>
		<td>
			<g:link action="show" id="${candidateInstance.id}">
			${fieldValue(bean: candidateInstance, field: "defaultVersion")}
			</g:link>
		</td>
		</tr>
	</g:each>