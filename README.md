# pg-clone-schema

Handles following objects:

* Tables - structure (indexes and keys) and optionally, data
* Views
* Materialized Views - Structure and data
* Sequences
* Functions/Procedures
* Types (composite and enum)
* Collations and Domains
* Triggers
* Permissions/GRANTs

Arguments:
* source schema
* target schema
* clone with data
* only generate DDL

You can call function like this to copy schema with data:
<br/>
>select clone_schema('development', 'development_clone', true, false);
<br/>

Alternatively, if you want to copy only schema without data:
<br/>
>select clone_schema('development', 'development_clone', false, false);
<br/>


