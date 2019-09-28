# exifTool-configs
Sample configuration file for EXIFTool for generating and embedding a PDF/A-compliant custom XMP Schema.

# Prerequisites:
The current version of ExifTool: https://sno.phy.queensu.ca/~phil/exiftool/. See the following note about naming and saving your config file, taken from the sample config file from the ExifTool documentation (https://sno.phy.queensu.ca/~phil/exiftool/config.html): 

"To activate this file, rename it to ".ExifTool_config" and place it in your home directory or the exiftool application directory.  (On Windows and Mac systems this must be done via the command line since the GUI's don't allow filenames to begin with a dot.  Use the "rename" command in Windows or "mv" on the Mac.)"

# XMP Extension Schemas in PDF/A

The config file I have provided here includes the necessary tag definitions to be able to embed a custom PDF/A-compliant XMP-Schema. This means defining the schema, namespace URI and prefix, as well as defining the properties (including their names, valueTypes, categories, and definitions). While it is also possible to define custom valueTypes, I have not tested this through this config file.

For more information, please see PDF Association's TechNote 0009: XMP Extension Schemas in PDF/A-1: https://www.pdfa.org/wp-content/uploads/2011/09/tn0009_xmp_extension_schemas_in_pdfa-1_2008-03-20.pdf

# This Example

This config file for EXIFTool has created an XMP extension based on PREMIS event metadata by creating xmp-premis namespace. For the initial test, I will be only be trying to implement limited Event metadata according to the PREMIS 3.0 Schema: http://www.loc.gov/premis/v3. 

