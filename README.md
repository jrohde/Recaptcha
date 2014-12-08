# ReCaptcha

## Installation

### Composer

Add the package to your require list:

        "require": {
            "studioforty9/recaptcha": "dev-master"
        }

Add the repository to your project composer.json file:

        "repositories": [
              {"type": "composer", "url": "http://packages.firegento.com"},
              {"type": "vcs", "url": "http://github.com/studioforty9/recaptcha"}
          ],

## Configuration

1. Once you've got the module installed, sign into your Google account and visit https://www.google.com/recaptcha.
2. Hit the "Get reCAPTCHA" link and you'll be taken to your account overview page. Register a new site by adding a label and any domains you want to allow for this specific reCAPTCHA widget.
3. Under 'Adding reCAPTCHA to your site' you should see 'Keys', specifically your 'Site Key' and 'Secret Key', copy and paste both keys into their respective configuration fields under 'System -> Configuration -> General -> ReCaptcha'.
4. Copy the /contacts/form.phtml template over to your theme, if you haven't already done so, just above the `buttons-set` div paste in the following code:

        <?php echo $this->getChildHtml('studioforty9.recaptcha.autorender'); ?>

## Contributing

Details to follow.

## Licence

MIT (see LICENCE file)