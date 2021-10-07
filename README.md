# open-tour-website

This website uses open-tour-website-lib (https://github.com/apothan/open-tour-website-lib) to create a tour and travel website using either the built in database that is created with open-tour or is able to connect to an outside OpenTour API.

## Requires:

```
Composer >= 2.0
NodeJS >= 12.13.0
```

## Installation:

```
git clone https://github.com/apothan/open-tour-website.git
composer install
yarn install
yarn encore dev
```

Update your .env file with your database credentials and create DB if needed

Update your .env file with your OpenTour API credentails

```
symfony server:start
```
And go to http://127.0.0.1:8000/

## Customisation:

You can overwrite each page 
- Copy the html.twig file from the vendor/apothan/open-tour-website-lib/templates folder
- Paste the file into templates/bundles/ApothanOpenTourWebsiteLib folder
- Chnage this file to how would like the website to look.

## Tips:

- If you are running this on Apache be sure to require the symfony apache pack:
```
composer require symfony/apache-pack
```
