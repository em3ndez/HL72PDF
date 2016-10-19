# HL72PDF // CDA2PDF // FHIR2PDF // XML2PDF

This is XML2PDF Renderer which is speacial build up for converting HL7 CDA and HL7 FHIR into PDF and embedding the xml file.
This Project is based on my HTMLConverter and the Apache Xalan Projekt.
You´ll find examples in the example.zip file.

#Run it
To run this Projekt simply set your JAVA_HOME and run
```
java -jar HL72PDF.jar [cda file] [xslt stylesheet] [output filename]
```

#Embed it
To embed this into you application simply add HL72PDF.jar to your classpath as library and call the static method convertToPDF(String cda_file, String stylesheet, String output_file)
```
HL72PDF.convertToPDF("C:/tmp/cda.xml", "C:/tmp/stylesheets/xda.xml", "MyPDFFile");
```

#Extract XML Attachement
Please use PDFBox PDDocumentNameDictionary Class and call getEmbeddedFiles()
https://pdfbox.apache.org/docs/2.0.2/javadocs/org/apache/pdfbox/pdmodel/PDDocumentNameDictionary.html
We will soon delopy an simple extractor
