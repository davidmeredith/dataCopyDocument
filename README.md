Data Copy Document XSD Schema
==============================
@author David Meredith

The XSD schema defines the <DataCopy> document root element that nests multiple 
<copy> operations. Each <copy> makes references to or nests in-line a data source and a data sink. 

* The schema uses both element-nesting and element-referencing to model relationships. 
Enabling both approaches reduces element repetition as multiple <copy> operations 
may reference the same shared resource(s) (e.g. common data source or sink definitions, 
common credentials etc). 

* The schema defines abstract elements to serve as extension points. This allows
import/extension of the base schema to define custom implementations of 
<abstractDataSource>, <abstractDataSink>, <abstractCredentials>, <abstractProperties>.  
See extendingSchemaExample.xsd and extendingDatacopyExample2.xml as an example. 

* See the datacopy.xsd for element documentation. 
