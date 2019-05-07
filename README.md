# exifTool-configs
Configuration files for EXIFTool

Testing a config file for EXIFTool to add PREMIS event metadata by creating xmp-premis namespace. For the initial test, I will be only be trying to implement limited Event metadata according to the PREMIS 3.0 Schema: http://www.loc.gov/premis/v3. 

The use case would be to copy some metadata from the xmp-pdf tags to the xmp-premis tags as well as fill in some default values. 

The initial test worked for adding xmp-premis: tags using EXIFTool, but the conformance for PDF/A failed due to the use of the XMP extension schema. The premis-event.xmp file attempts to overcome that by following the convention for designing an xmp extension schema.

Further steps have included updating the exiftool config file in order to be able to write the user defined extension in a way that conforms to PDF/A to the file. See the documentation for examples and see commands.txt for some of the exiftool commands used.
