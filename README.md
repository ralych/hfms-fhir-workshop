# hfms-fhir-workshop

## HL7 FHIR Testserver
### FHIR Server der HAPI (Java Library) Entwicklung
#### Capability Statement
[CapabilityStatement JSON Format](http://hapi.fhir.org/baseR4/metadata?_format=json)<br>
[CapabilityStatement XML Format](http://hapi.fhir.org/baseR4/metadata?_format=xml)

###FHIR Server CH-Core
#### Capability Statement
[CapabilityStatement JSON Format](http://test.ahdis.ch/r4/metadata?_format=json)
[CapabilityStatement XML Format](http://test.ahdis.ch/r4/metadata?_format=xml)


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
Validieren Patient Resource gegen CH-Core<br>
POST http://test.ahdis.ch/r4/$validate?profile=http://fhir.ch/ig/ch-core/StructureDefinition/ch-core-patient<br>
[body](https://github.com/ralych/hfms-fhir-workshop/resources/fhirch/)


Some scripts can be found [here](https://github.com/ahdis/matchbox/blob/master/test.ahdis.ch.http)




