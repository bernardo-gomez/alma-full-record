# get_alma_record
Python-based webservice that receives an Alma mms_id or an item barcode and
produces a string that contains the bibliographic record and items.
the string could have one of three formats:
  - xml ( MARCXML)  , or
  - marcedit ( terry reese's marcEdit application), or
  - text ( bernardo gomez format).
  example:
   https://kleene.library.emory.edu/cgi-bin/get_alma_record?doc_id=990024996580302486&format=marcedit 

**Files**: 
   - get_alma_record.py , the main script;
   - get_alma_record.cfg , the configuration file.

**get_alma_record** retrieves bibliographic and holding information from 
ALMA via ALMA API requests.
the item information is displayed as a "999" MARC field.
