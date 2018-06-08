# Signature::Pad::Rails

Thomas Bradley's Signature Pad! For Rails! So great.

This gem provides:

  * Signature Pad 2.5.2 (js, css, font, and cursor)
  * flashcanvas.js (js and swf)
  * json2 (js)
  
The versions of flashcanvcas and json2 are as provided with the original Signature Pad package.

To read more about Signature Pad, see http://thomasjbradley.ca/lab/signature-pad/. The Signature Pad source code
is at https://github.com/thomasjbradley/signature-pad. If you wish to make changes to Signature Pad itself,
fork Thomas Bradley's Signature Pad project and contribute your changes back to that project.


## Installation

Add this line to your application's Gemfile:

    gem 'signature-pad-rails'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install signature-pad-rails

After installing the gem, add the following to your application.js:

    //= require signature-pad

Or, you may instead add any of the individual javascript components:

    //= require signature-pad/jquery.signaturepad
    //= require signature-pad/flashcanvas
    //= require signature-pad/json2

And optionally add to your application.css:

    *= require signature-pad

The css will include the custom cursor and font. The cursor and font are included in assets, and if you wish to
access them manually rather than using the signature-pad css, you may do so using the asset_path helper, eg:

    cursor: url(<%= asset_path 'signature-pad/pen.cur' %>) 16 16, crosshair;

or

    src: url("<%= asset_path 'signature-pad/journal.eot' %>");


## Requirements

signature-pad-rails requires:

* rails 3.x, 4.x, or 5.x
* jquery-rails 3.0.0 or greater


## Usage

See the Signature Pad documentation at http://thomasjbradley.ca/lab/signature-pad/.


## Credits

The rails gem is written and maintained by [Justin Tomich](https://github.com/tomichj).

Signature Pad is written by [Thomas J Bradley](http://thomasjbradley.ca).

json2.js is written by [Douglas Crockford](http://www.json.org/js.html).

FlashCanvas is written by the [FlashCanvas Project](http://flashcanvas.net/). 


## Contributing

Contributions are very welcome. Fork and push a change request. Thanks!
