# Organizational Structure

The organization shall be directed by three boards:

1. The _**Board of Strategy**_ shall define the strategic goals of the organization. It shall be componed of a _**Director of Planning**_, a _**Director of Execution**_, and a _**Director of Oversight**_. It be led by the _**Director of Planning**_.
2. The _**Board of Execution**_ shall direct the execution of the strategic goals of the organization and shall be led by the _**Director of Execution**_.
3. The _**Board of Oversight**_ shall ensure that the organization is adhering to our Core Values and applicable internal and external laws. It shall be led by the _**Director of Oversight**_.


```mermaid
---
config:
  layout: elk
---
graph LR
	bos[Board of Strategy]
	boe[Board of Execution]
	boo[Board of Oversight]

	bos --> boe --> boo --> bos
	bos --> boo --> boe --> bos
```

```mermaid
graph
	subgraph bos[Board of Strategy]
		dPlan[Director of Planning]
		dExec[Director of Execution]
		dPeople[Director for the People]
	end
	dPlan --> dExec --> dPeople --> dPlan
	
	subgraph boe[Board of Execution]
		dRes[Director of Resources]
		dKnow[Director of Knowledge]
		dHealth[Director of Health]
		dArt[Director of Art and Culture]
	end

	subgraph boo[Board of Oversight]
		dLaw[Director of the Law]
		dJud[Directory of the Judiciary]
		dAud[Director of Audits]
	end

	bos --> boe --> boo --> bos

	dExec --> boe
	dPeople --> boo

	dRes --> Environment
	dRes --> Food
	dRes --> Shelter
	dRes --> Energy
	dRes --> Luxuries

	Environment --> Water
	Environment --> Land
	Environment --> Air
	Environment --> Extraterrestrial

	Food --> Agriculture

	dKnow --> Science
	dKnow --> Education
	dKnow --> Communication

	Science --> History
	Science --> Medicine

	dHealth --> Mental
	dHealth --> Physical
	dHealth --> Safety

	Physical --> Disability

	dArt --> Parks
	dArt --> Recreation
	dArt --> Monuments
```
