SendGrid on Google App Engine
======================

This git repository helps you to send emails quickly and easily through SendGrid on Google App Engine using PHP.


Running on Google App Engine
----------------------------

Create an SendGrid account at http://sendgrid.com/pricing.html

Create an account at https://appengine.google.com/ and set up your local machine with the client tools https://developers.google.com/appengine/docs/php/gettingstarted/installing

Create an application at https://appengine.google.com/start/createapp

Clone SendGrid application on your local machine
<pre>
    git clone https://github.com/sendgrid/google-php-sample-app
</pre>

###Configuration###

Configure `index.php` file with your information:

Update the *&lt;sendgrid_username&gt;* and *&lt;sendgrid_password&gt;* with your SendGrid credentials.
```php
    $sendgrid_username = '&lt;sendgrid_username&gt;';
    $sendgrid_password = '&lt;sendgrid_password&gt;';
```
Update the *&lt;from_address&gt;* with your email address
```php
    $from_email = "&lt;from_address&gt;";
```
Update application identifier in `app.yaml` file
```yaml
    application: application_identifier
```

Upload your application to Google App Engine: https://developers.google.com/appengine/docs/php/gettingstarted/uploading

That's it, you can now checkout your application at:
<pre>
    http://application_identifier.appspot.com/
</pre>




