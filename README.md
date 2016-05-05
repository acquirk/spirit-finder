Spirit Finder

About
Spirit Finder is a javascript library built on an open-source library by Google Maps. It can be used by breweries, distilleries, wineries, and other craft brands as a website plugin. 

On the frontend, the goal is to allow customers to easily find your products wherever they are.

On the backend, the goal is to allow marketing or sales directors to upload placement data from their distributors and have it automatically populate the Spirit Finder page on their live website.


Info
Here is the Google Maps js-store-locator library:
https://github.com/googlemaps/js-store-locator

And here is the example I pulled from:
https://googlemaps.github.io/js-store-locator/examples/panel.html

Here is my current implementation:
http://cardinalspirits.com/spirit-finder

The JS starts at line 80 on that page, if you want to dig through the javascript files (all hosted at assets.cardinalspirits.com, an apache webserver I host at Dreamhost).

The static CSV is loaded from http://assets.cardinalspirits.com/spirit-static-ds.js

The static CSV lives here: http://assets.cardinalspirits.com/cs-placements-test.csv

Current status: not working

I changed a few variables in the spirit-static-ds.js file from Medicare and Audio, to Coffee and Vodka. 

Fixed: Cross-domain permissions issue (used .htaccess to solve)

Reference:

JS-Store-Locator reference:
https://googlemaps.github.io/js-store-locator/reference.html

Building a store locator application with the Google Maps API and Google Cloud SQL:
https://storage.googleapis.com/support-kms-prod/C4EA761B96A0D8EA170411A34ACE3BB7C9C1



Future Development
Ideally there would be an upload mechanism that parses the data from a CSV and associates each column with an associated database field. This would alleviate potential issues with reformatting CSV data from different distributors, since it is unlikely that placement reports from different distributors would have the same column headings. 

