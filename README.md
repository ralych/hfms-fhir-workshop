# hfms-fhir-workshop

## HL7 FHIR Testserver
### FHIR Server der HAPI (Java Library) Entwicklung
#### Capability Statement
[CapabilityStatement JSON Format](https://hapi.fhir.org/baseR5/metadata?_format=json)<br>
[CapabilityStatement XML Format](https://hapi.fhir.org/baseR5/metadata?_format=xml)

#### CRUD Patient
CREATE:
POST http://hapi.fhir.org/baseR4/Patient<br>
[body](https://github.com/ralych/hfms-fhir-workshop/resources/hapi/POST_Patient_MustermannMax.json)

READ:
GET http://hapi.fhir.org/baseR4/Patient/1710296<br>
no body

UPDATE:
PUT 		<br>
[body](https://github.com/ralych/hfms-fhir-workshop/resources/hapi/PUT_Patient_1710296_gender-male.json)
<br>or<br>
[body](https://github.com/ralych/hfms-fhir-workshop/resources/hapi/PUT_Patient_1710296_gender-male.json)

DELETE:
DELETE http://hapi.fhir.org/baseR4/Patient/2040998<br>
no body

#### CRUD Practitioner

#### CRUD Organization

#### CRUD PractitionerRole

#### CRUD Observation


#### Searching
Search Patient by family and given<br>
GET http://hapi.fhir.org/baseR4/Patient?given=Peter&family=Balm

Search Observations for Patient|Author...


<br>
#### Validate Resource against profile
https://validator.fhir.org/
Bsp. Ressourcen: https://github.com/ralych/hfms-fhir-workshop/resources/fhirch/

