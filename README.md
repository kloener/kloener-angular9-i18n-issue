# Angular9 i18n issue with multiple HTML tags in target.

This is a minimal sample project to emphasize and show the issue with i18n since Angular v9 when more HTML tags are used inside "target" than in "source".

## Build & Run


* `npm install`
* `npm build:localize`
* browse to [http://localhost:4205/de-DE](http://localhost:4205/de-DE) -> invalid HTML tag order
* browse to [http://localhost:4205/en-GB](http://localhost:4205/en-GB) -> just text changes added
* browse to [http://localhost:4205/de](http://localhost:4205/de) -> source text

You can try to run `docker run -it -p4205:80 -v $(pwd)/dist/kloener-angular9-i18n-issue:/app --workdir /app --rm php php -S 0.0.0.0:80` 
or run an http-server on dist with anything else.
