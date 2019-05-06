C:\exiftool-11.32\exiftool.exe -XMP-pdfaExtension:schemasProperty="{name=EventType, valueType=Text, category=internal, description=Event Types according to LOC}" \filePath\fileName.pdf
C:\exiftool-11.32\exiftool.exe -XMP-pdfaExtension:schemasProperty+="{name=EventDateTime, valueType=Date, category=internal, description=Date digitized}" \filePath\fileName.pdf
C:\exiftool-11.32\exiftool.exe "-XMP-premis:EventDateTime<FileCreateDate" "-XMP-premis:EventType=migration" \filePath\fileName.pdf
