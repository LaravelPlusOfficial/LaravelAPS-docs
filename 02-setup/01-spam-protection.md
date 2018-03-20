<h1 class="fsz-xl tt-u ls-16">Spam Protection</h1>
LaravelAPS has built in spam protection.

<h2 class="fsz-lg tt-u ls-16 c-gray mt-6 bdB">Akismet</h2>
LaravelAPS uses akismet api for spam protection. Go to [Akismet webiste](https://akismet.com) and get the api key to use. Don't forget to add your site. you can even add your `domain.test` site. Use that key and put into the following keys in `.env` file

    AKISMET_APIKEY= 
    AKISMET_BLOGURL=https://domain.test


<h2 class="fsz-lg tt-u ls-16 c-gray mt-6 bdB">Google recaptcha</h2>
We use [Google Recaptcha](https://www.google.com/recaptcha/admin#list) to verify human. Go to Google Recaptcha website and get site key and site secret and fill into into the following keys in `.env` file.

    GOOGLE_RECAPTCHA_SITE_KEY=
    GOOGLE_RECAPTCHA_SECRET_KEY=
