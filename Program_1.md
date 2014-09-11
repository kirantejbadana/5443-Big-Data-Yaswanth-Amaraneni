### CONVERT CSV TO JSON

I choose python ,why?, because server side files has significant data(in csv format) to render that data(into json format) and which is used by clients and python can easily convert data and tables from spread sheet which is in CSV format to JSON format.

here is sample code...
```
import csv
import json

f = open( 'sample.csv', 'r' )
reader = csv.DictReader( f)
out = json.dumps( [ row for row in reader ] )
print out
```
source : http://ntare16.wordpress.com/2012/01/26/python-code-to-convert-csv-to-json/

I chose CSV file because it has flat data as JSON. So Its easy to convert CSV to JSON.

| Type | Description                                  | Size    |Compressed size|   %   |
|------|----------------------------------------------|---------|---------------|------:|
| csv  |Comma seperated values                        | 484MB   |     59MB      | 87.8  |
| sql  |Structured Query Language (insert statements) | 467MB   |     60MB      | 87.1  |
| xml  |EXtensible Markup Language                    | 2.3GB   |     75MB      | 96.7  |
| yaml |Yet Another Markup Language                   | 771MB   |     61MB      | 92.0  |
| json |Javascript Object Notation                    | ?       |               |       |

** % means that much of percentage compressed compare to original size.
