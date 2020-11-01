# 1st-PyCrawlerMarathon

## Day 001 - data format & file I/O
* Get file from given url (library urllib.request): [urllib.request.urlretrieve(url, filename=None, reporthook=None, data=None)](https://docs.python.org/3.6/library/urllib.request.html?highlight=urlretrieve#urllib.request.urlretrieve)
* Open file: [open(file, mode='r', buffering=-1, encoding=None, errors=None, newline=None, closefd=True, opener=None)](https://docs.python.org/3.6/library/functions.html?highlight=open#open)
    * Return a file object
    * Use `with open() as f:` to automatically manage the file object
    * Read/Write member functions of file object:
        * Read: read(), readline(), readlines()
        * Write: write(), writelines()
* Detect file encoding (library [chardet](https://github.com/chardet/chardet)): [chardet.detect(byte_str)](https://chardet.readthedocs.io/en/latest/api/chardet.html#chardet.detect)

## Day 002 - process .csv file
* Parse .csv file (library csv): [csv.reader(csvfile, dialect='excel', **fmtparams)](https://docs.python.org/3.6/library/csv.html?highlight=csv%20reader#csv.reader)

## Day 003 - process .xml file
* Basic: [xml.dom.minidom.parse(filename_or_file, parser=None, bufsize=None)](https://docs.python.org/3.6/library/xml.dom.minidom.html#xml.dom.minidom.parse)
* Friendly: [xml.etree.ElementTree.parse(source, parser=None)](https://docs.python.org/3.6/library/xml.etree.elementtree.html?highlight=xml%20etree%20elementtree#xml.etree.ElementTree.parse)
* To dict ([xmltodict](https://github.com/martinblech/xmltodict)): dict( xmltodict.parse( xml_string ) )
