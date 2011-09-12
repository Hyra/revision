Revionable Behavior

Courtesy of the CakePHP-Assets made by Alkemann at [CakePHP-Assets](https://github.com/alkemann/CakePHP-Assets/ "CakePHP-Assets")

## Install
Clone this plugin to `app/plugins/revision`

Add the following to either `app_model.php` or a specific model you want to keep Revisions of:
  public $actsAs = array('Revision.Revision');

Create a shadow table for the models you want to keep revisions of.
Duplicate the table (not the contents) and:
- Remove the PRIMARY key from the `id field`
- Add a field `version_id` with PRIMARY KEY and `auto_increment`
- Add a field `version_created` as DATETIME

## Todo
Extend this README :)