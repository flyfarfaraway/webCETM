# Toolset Common Library

## 2.5.8
* New admin notice about Types becoming commercial

## 2.5.7
* (toolsetcommon-305) Improve the database structure for relationships and associations.
* (types-1213) Implement a mechanism for handling database integrity issues within the m2m API.
* (types-1265) Introduce a QUERY_HAS_TRASHED_POSTS argument to Toolset_Association_Query
* Many improvements to the m2m API, especially to the relationship query.
* (toolsetcommon-328) Enforce cardinality limits when creating associations between two elements.
* (toolsetcommon-330) Prevent upgrade routines from running repeatedly. Fix a m2m activation issue.
* (toolsetcommon-249) The Toolset_Twig_Autoloader now bails out when it's possible to load the Twig_Environment class. 

## 2.5.6
* Fixed a but that prevented CRED attributes offered as select2 instances from getting their values in the final shortcode.

## 2.5.5
* Released with Types 2.2.20 and Views 2.5.1
* Fix the way we determine whether the m2m API should be enabled on fresh sites without post relationships by default (types-1252).
* Fix several compatibility issues with Visual Composer.
* Fix a problem when gathering the title of some Types fields.

## 2.5.4
* Released with CRED 1.9.3
* Include a shared Toolset JS shortcodes library.
* Fixed a problem with loading the latest Bootstrap CSS Components from Toolset Common.
* Fixed some notices caused by slightly different array structures on fields.

## 2.5.3
* Released with Types 2.2.17

## 2.5.2
* Released with Views 2.5 and Layouts 2.1

## 2.5.1
* Moved Twig from Types to the Toolset Common Library (toolsetcommon-63).
* Created an abstraction of a listing page in the Toolset Common Library (toolsetcommon-64).
* Added an extendable Toolset Troubleshooting page (toolsetcommon-76).
* Implemented a generic upgrade mechanism (toolsetcommon-75).
* Moved classes related to Types fields to the library (toolsetcommon-84, toolsetcommon-104).
* Fix a minor issue with search while not on first page of the listing in Field Control and Custom Fields pages in Types (toolsetcommon-178)
* Implemented the m2m API (toolsetcommon-70).

## 2.5.0
- Added the ability to control the settings from selected themes.

## 2.4.5
- Compatibility with Types 2.2.16 and the new admin notice asking users to register their commercial plugins.

## 2.4.4
- Compatibility with CRED 1.9.2

## 2.4.3
- Compatibility with Types 2.2.14, Vies 2.4.1, CRED 1.9.1, Access 2.4.2 and Layouts 2.0.2

## 2.4.2
- Removed notices, which leads to documentation of integration between Layouts and 3rd party themes.

## 2.4.1
- Removed notices, to push users to activate Layouts theme integration plugins based on the current theme.
- Added filter to remove/add automatic notices on demand.

## 2.4.0
- Updated Font Awesome library to 4.7.0
- Included a mechanism to insert Bootstrap grid rows into selected Toolset editors.
- Included the needed changes for providing Bootstrap compatible output to CRED frontend forms.
- Improved the shared admin notices so they only get displayed for admins.
- Included the Chosen library as alternative to select2.
- Fixed an issue with a missing CRED datepicker stylesheet.
- Fixed an issue with link elements of Visual Composer when used as editor in Content Templates.
- Moved a CSS rule regarding jQuery UI datepicker, that was removed from Types.


## 2.3.2
- Fixed localization issue with date field and WordPress below 4.7
- Most notices are now only shown to Administrators.

## 2.3.1

- Improved the styling for CRED file-related fields.
- Fixed some compatibility issues with PHP 7.1
- Fixed taxonomy suggestions on CRED forms.

## 2.3.0

- Various fixes and adjustments for CRED 1.8.6
- Adds callback methods for wpPointer object onOpen and onClose
- Allows user to ask Toolset to load Bootstrap library for them, or alternatively set the Bootstrap version they are using on their own
- layouts-1239: Added Toolset_Admin_Notice_Layouts_Help
- Extend the post objects relationships management with two actions to gather data on demand.
- Only include the jQuery datepicker stylesheet on demand when the current page contains a datepicker from Toolset.
- Include the user editors in the common bootstrap class.
- toolsetcommon-127, toolsetcommon-55: Include knockout.js
- toolsetcommon-139: Clean up Toolset_Assets_Manager and define constants for asset handles 
- toolsetcommon-144: Added Toolset_Admin_Notices_Manager
- toolsetcommon-137: Make the toolset-forms classes autoloaded.
- toolsetcommon-72: Implemented a classmap-based autoloader for all Toolset plugins.
- toolsetcommon-140: Improve a way to detect the status of WPML.
- toolsetcommon-142: Use get_user_locale() instead of get_locale() if it's available.

## 2.2.10

- types-1045: Do not assume field value type in Enlimbo_Form::textfield().

## 2.2.9

- Fix a validation issue for file, audio, video and embed fields affecting Types. 
  Allow URLs with non-latin characters, but only for URLs that point to attachments
  from the Media Library (validated by WordPress media upload mechanism) (types-1013).
- Improve the validation for non-required Skype fields (toolsetcommon-128).

## 2.2.6

- Fix a CRED issue with added validation rules (types-988).
- Handle several issues related to using "0" as a default field value and saving it to the database (toolsetcommon-106).
- Minor compatibility fixes for the upcoming CRED 1.8.4 release.
- Extend WPToolset_Cake_Validation with the "url2" validation as a counterpart to the validation method in JQuery UI (types-988).

## 2.2.5 (November 5, 2016)
 
- Thorough check for security vulnerabilities.

## 2.2.4 (November 2, 2016)

- Fixed a problem with some assets management by defining better rules on constant definitions.

## 2.2.3 (October 10, 2016)

- Fixed select2 edge cases when methods are called on non-select2 initialised element.
- Refined special handling of old inputs by making sure target is only a select and not the hidden relative element
- Extended the valid date formats that Types and CRED supports for the Date field.

## 2.2.2 (September 26, 2016)

- Updated the bundled select2 script to version 4.0.3
- Fixed a problem with some assets URLs lacking a backslash
- Improved management of CRED file fields uploads
- Improved the frontend markup for CRED taxonomy fields
- Added an internal Toolset compatibility class

## 2.2.1 (August 25, 2016)
 
- Avoid translating the Toolset top level admin menu label
	
## 2.2 (August 24, 2016)

- Added compatibility classes for Relevanssi and Beaver Builder
- Added a CSS components class
- Improved the Toolset Common assets management
- Added the Glyphicons library

## 2.1 (June 13, 2016)

- Refactored event-manager library to toolset-event manager to namespace it and avoid conficts with ACF Plugin
- Added a new class for promotional and help videos management
- Improved compatibility with PHP 5.2
- Improved compatibility with WPML, including admin language switchers and loading times
- Improved compatibility for CRED file uploads and bundled scripts
- Fixed double slashes on assets URLs

## 2.0 (April 7, 2016)

- Created new loader to load resources for all plugins when plugin loads
- Refactored in a more organised way files and resources to be compatible with the new loader
- Added scripts and styles manager class to register and enqueue static resources with a unified system
- Added Toolset Dialog Boxes to provide a unified way to create and render dialogs
- Fixed various bugs

## 1.9.2 (March 17, 2016)
  
- Fixed issue in validation messages on Amazon S3

## 1.9.1 (March 15, 2016)
  
- Added control to filter array to prevent exceptions
- Prevented error when object does not have property or key is not set in array filter callback
- Fixed glitch in validation library
- Absolute path to include toolset-forms/api.php
- Fixed search terms with language translation

## 1.9 (February 15, 2016)
  
- Tagged for Types 1.9, Views 1.12, CRED 1.5, Layouts 1.5 and Access 1.2.8
- Updated parser.php constructors for PHP7 compatibility.
- Updated the adodb time library for PHP7 compatibility.
- Introduced the Shortcode Generator class.
- New utils.

## 1.8 (November 10, 2015)
  
- Tagged for Views 1.11.1, Types 1.8.9 and CRED 1.4.2
- Improved the media manager script.
- Added helper functions for dealing with $_GET, $_POST and arrays.
- Improved CRED file uploads.
- Improved taxonomy management in CRED forms.
- Improved usermeta fields management in CRED forms.

## 1.7 (October 30, 2015)
  
- Tagged for Views 1.11 and Layouts 1.4

## 1.6.2 (September 25, 2015)
 
- Tagged for CRED 1.4, Types 1.8.2

## 1.6.1 (August 17, 2015)
  
- Tagged for Composer Types 1.8, Views 1.10, CRED 1.4 and Layouts 1.3

## 1.6 (June 11, 2015)
  
- Tagged for Types 1.7, Views 1.9 and Layouts 1.2

## 1.5 (Apr 1, 2015)
  
- Tagged for Types 1.6.6, Views 1.8, CRED 1.3.6 and Layouts 1.1.
- Fixed issue when there is more than one CRED form on a page with the same taxonomy.
- Fixed a little problem with edit skype button modal window - was too narrow.
- Fixed empty title problem for filter "wpt_field_options" on user edit/add screen.
https://wp-types.com/forums/topic/populate-select-field-in-wpcf-um-group/
- Added filter "toolset_editor_add_form_buttons" to disable Toolset buttons on the post editor.
- Added placeholder attributes to fields.
- Updated CakePHP validation URL method to allow new TLD's.

## 1.4 (Feb 2 2015)
  
- Tagged for Views 1.7, Types 1.6.5, CRED 1.3.5 and Layouts 1.0 beta1
- Updated Installer to 1.5

## 1.3.1 (Dec 16 2014)
  
- Tagged for Views 1.7 beta1 and Layouts 1.0 beta1
- Fixed issue about Editor addon and ACF compatibility
- Fixed issue about branding loader

## 1.3 (Dec 15 2014)
  
- Tagged for Views 1.7 beta1 and Layouts 1.0 beta1
