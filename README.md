# Partial Text from PDF (PTFP)

### PTFP is a JS/HTML tool for extracting text from only certain pages of a text based pdf.

##### I created this as part of a larger project ([ReListed](https://relistedonline.com)) with the goal of extracting text client side rather than sending a file to a server to be processed, saving a round trip and sidestepping the potential risks of a file upload. PTFP makes use of pdfjs, and as such should be secure from XSS vulnerabilities, but the extracted text is not currently being sanitized, as I handle that on the server in production.

### Aren't there a million of these on the internet?

#### Yes, but I decided to share this on github after three realizations.
##### 1. I really don't want to accept file uploads. The exploitation potential is enormous, and the validation is a nightmare!
##### 2.  They all seem to upload files to their servers, and I don't want to simply take their word that they my potentially sensitive files are getting deleted, not being read, and not being used to train AI.
##### 3.  They all seem to be using OCR. OCR is very good at its job, but the option for getting the raw text is nice to have.

### Getting Started
#### Simply download the html file and open it in a web browser! Note that you'll need an internet connection as pdfjs is delivered via CDN.

#### Feel free to fork this project.
