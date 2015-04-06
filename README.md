Obtain tracking information for your packages, as well as create and print shipping labels.

Note: This version has primarily been tested with US-based addresses.

### Typical usage scenario

This connector will allow you to check the status of a package by supplying the tracking number. It will also allow you to create shipping labels, buy inputting the necessary information (shipper details, recipient details, package details, etc.)

### Features and limitations

* Must have an account with UPS to utilize their API. For more information, you can visit: https://www.ups.com/upsdeveloperkit

### Dependencies

* Mendix Business Modeler 5.14.1+
* Community Commons module

### Installation

* Download the UPS Connector module
* Download the Community Commons module

### Configuration

* Update the following constants with your UPS Developer information:
 * Username (Track and Ship)
 * Password (Track and Ship)
 * Url (Track and Ship)
 * AccessKey (Track and Ship)
 * AccountNumber (Ship only)
* Two pages have been created for quick testing or a starting point to add to your app:
 * TrackingInfo
 * ShippingLabel
* When creating a shipping label, please note the following:
 * Only Phone Extension is optional
 * Phone Number can be either numeric or alpha-numeric
 * State and Country require its two-character abbreviation
* Regarding default values in the shipping label request:
 * The values can be updated accordingly or made configurable, but the current default values represent the basic configuration for creating shipping labels. Further details regarding these values and options can be found at the UPS Developer site: https://www.ups.com/upsdeveloperkit
* Regarding printing shipping labels:
 * By default, a PDF will be generated containing the embedded shipping label image
 * The width of the dynamic image has been set to provide optimal appearance in conjunction with the default PPI of the document template (120), but this can always be updated to any desired configuration


