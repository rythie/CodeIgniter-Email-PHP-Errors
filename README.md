# CodeIgniter-Email-PHP-Errors


A configurable drop-in customization to email yourself PHP errors encountered in your application.

## Usage

1. drop ```email_php_errors.php``` into ```application/config``` and ```MY_Exceptions.php``` into ```application/core```. If you already have a ```MY_Exceptions.php``` just modify accordingly.
2. Edit the config file with your from email and to email, the subject line, and the message template.
3. Add $this->_error =& load_class('Exceptions', 'core'); $this->_error->send_exceptions(); to your controllers

## Change Log

**1.0.1**

* added enable/disable config item
* parses subject *and* content for short codes

**1.0.0**

* initial release
