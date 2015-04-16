# sfJqueryDateTimePlugin

jQuery select date and time plugin for Symfony 1.4

##  Git

Git submodule add:

	$ git submodule add https://github.com/northway/sfJqueryDateTimePlugin.git plugins/sfJqueryDateTimePlugin

Git submodule update:

	$ git submodule update --remote

## Install

You need to add this line to ProjectConfiguration.class.php:

    $this->enablePlugins('sfJqueryDateTimePlugin');

Publish assets:

    php symfony plugin:publish-assets

Then a Symfony cache clear:

    $ php symfony cc

## Usage

  view.yml

    default:
      stylesheets:
        - /sfJqueryDateTimePlugin/css/jquery.datetimepicker.css
      javascripts:
        - /sfJqueryDateTimePlugin/js/jquery.datetimepicker.js

## Example

	HTML:
		
		<input id="datetimepicker" type="text" >

	JavaScript:

		jQuery('#datetimepicker').datetimepicker();

For more exmaples: http://xdsoft.net/jqplugins/datetimepicker/

If you run into some error, check symfony logs and script logs.

If you think you can improve this plugin or found some error, feel free to fork and create a pull request.
