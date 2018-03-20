<h1 class="fsz-xl tt-u ls-16">Environment Variables</h1>
LaravelAPS has environment variables located in `.env` file. As a starter `.env.example` file is provided. It's pretty standard with all the laravel installation. You need to get the required values for keys present in `.env` file. Following are the default keys which are present in `.env` file

<h2 class="fsz-lg tt-u ls-16 c-gray mt-6 bdB">Example Environment File</h2>
These keys are default keys. 

    APP_NAME="LaravelAPS"
    APP_ENV=local
    APP_KEY=
    APP_DEBUG=true
    APP_LOG_LEVEL=debug
    APP_URL=http://localhost:8000
    APP_TIMEZONE="America/Toronto"
    
    LOG_CHANNEL=stack
    
    MAIL_FROM_ADDRESS="hello@example.com"
    MAIL_FROM_NAME="${APP_NAME}"
    
    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=xxxxxxxx
    DB_USERNAME=xxxxxxxx
    DB_PASSWORD=xxxxxxxx
    
    AKISMET_APIKEY=xxxxxxxx
    AKISMET_BLOGURL="https://example.com"
    
    BROADCAST_DRIVER=log
    CACHE_DRIVER=file
    SESSION_DRIVER=file
    SESSION_LIFETIME=120
    QUEUE_DRIVER=sync
    
    REDIS_HOST=127.0.0.1
    REDIS_PASSWORD=null
    REDIS_PORT=6379
    
    MAIL_DRIVER=smtp
    MAIL_HOST=smtp.mailtrap.io
    MAIL_PORT=2525
    MAIL_USERNAME=
    MAIL_PASSWORD=
    MAIL_ENCRYPTION=TLS
    
    PUSHER_APP_ID=
    PUSHER_APP_KEY=
    PUSHER_APP_SECRET=
    PUSHER_APP_CLUSTER=mt1
    
    MIX_PUSHER_APP_KEY="${PUSHER_APP_KEY}"
    MIX_PUSHER_APP_CLUSTER="${PUSHER_APP_CLUSTER}"
    
    # Test keys
    GOOGLE_RECAPTCHA_SITE_KEY=
    GOOGLE_RECAPTCHA_SECRET_KEY=
    
    GITHUB_CLIENT_ID=
    GITHUB_CLIENT_SECRET=
    SOCIALITE_GITHUB_CALLBACK="/socialite/github/callback"
    
    TWITTER_CLIENT_ID=
    TWITTER_CLIENT_SECRET=
    TWITTER_ACCESS_TOKEN=
    TWITTER_ACCESS_SECRET=
    SOCIALITE_TWITTER_CALLBACK="/socialite/twitter/callback"
    
    FACEBOOK_APP_ID=
    FACEBOOK_APP_SECRET=
    SOCIALITE_FACEBOOK_CALLBACK="/socialite/facebook/callback"
    
    GOOGLE_CLIENT_ID=
    GOOGLE_CLIENT_SECRET=
    GOOGLE_SERVER_KEY=
    SOCIALITE_GOOGLE_CALLBACK="${APP_URL}/socialite/google/callback"

<h2 class="fsz-lg tt-u ls-16 c-gray mt-6 bdB">Install Command</h2> 
Though you can install and config LaravelAPS by your own, but we have also provided install command to get you started asap. To use that command just run following command.

    php artisan aps:install
    
It will ask you value for each environment key and fill it to `.env` file, so that you don't have to do it manually. If you have values for the .env keys, you can put it on, but if not just delete `.env` file clear your database and run the above command again.

<h2 class="fsz-lg tt-u ls-16 c-gray mt-6 bdB">Install Passport</h2>
LaravelAPS uses [Laravel Passport](https://github.com/laravel/passport) for OAuth2 server authentication. To get authentication working properly you need to install passort keys by running following command

    php artisan passport:install
    
<h2 class="fsz-lg tt-u ls-16 c-gray mt-6 bdB">Serve the site</h2>
To run app in development, you can use [Laravel Valet](https://github.com/laravel/valet) or can run following command to run app at localhost `http://localhost:8000`

    php artisan serve
    
    

        