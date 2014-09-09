CONVERTING CSV TO JSON

I choose python ,why?, because server side files has significant data(in csv format) to render that data(into json format) and which is used by clients.

here is sample code...

import csv
import json

f = open( 'sample.csv', 'r' )
reader = csv.DictReader( f)
out = json.dumps( [ row for row in reader ] )
print out

source : http://ntare16.wordpress.com/2012/01/26/python-code-to-convert-csv-to-json/

I choose CSV file because it has flat data as JSON.
