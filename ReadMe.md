# nirmitee.io Recruitment Task

To parse XML export of Tally's transactions and convert it into `.xlsx` file according to template <!--(which, hopefully, is generated by one of Tally's softwares)--> `2-output.xlsx` **only for voucher type "Receipt"**. (and it seems `0-raw.xlsx` is a possible *represnetation* of what Tally'd see for the given input XML)

## Ways to standout

 * create [ReST] API to generate result
  * query string for recipt and other voucher types?
  * 2xx and 4xx error codes
 * optimization
  * NOTE: avoid until confident about correctness
 * robust code

## How to use?

Please ensure to install all dependencies via requirements.txt

 1. provide path to input xml via cli e.g. `python parse.py spec/1-input.xml`, or
 2. spin up server with `uvicorn server:app --reload` and visit `localhost:8000/docs`, find green colored POST button there, insert properly formatted (" escaped, etc.) in request body and wait for the response.
