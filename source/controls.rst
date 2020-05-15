.. sectionauthor:: Mikhail Gusev <mikhail.gusev@nextgis.ru>

.. _ngfb_controls:

Form controls
==============

Tabs
-------

Tabs grouping for other elements.

Properties:

* **Current page**. Current page which should be displayed by default.
* **Headers**. A list of header strings.

Date & time
------------

An element which allows to pick a date, time or date&time value.

Properties:

* **Is current**. Automatically assigns current value during the data collecting process. Otherwise user will be able to pick it manually.
* **Type**. Type.
* **Initial value**. Initial fixed date/time value.
* **Keep last value**. Whether to keep last entered value for this element during data collecting process.

Distance meter
---------

This element automatically measures distance between current position of the point and current position of the surveyor.

Dependent comboboxes
----------------

A pair of drop-down lists with predefined items. The item list of the dependent combobox depends on the items of the main combobox.

Properties:

* **Items**. Lists of items for both comboboxes.
* **Keep last value**. Whether to keep last entered value for this element during data collecting process.

Coordinates
----------

An element which automatically saves current geographical coordinates in text format.

Properties:

* **Is hidden**. Do not show this element. The coordinates will be written to the layer's field(s) anyway.
* **CRS**. Coordinate Reference System.
* **Format**. The format of the string which will be written to the layer's field(s).

Label
-------

An element which displays static text

Properties:

* **Text**. Displayed text.

Signature field
-------

A field for signature.

Void space
------

Void space for making indents.

Radiogroup
-----------

A list with predefined items which allows the selection of only one value.

Properties:

* **Keep last value**. Whether to keep last entered value for this element during data collecting process.
* **Items**. A list of items (must have at least two items).

Splitted combobox
----------------

A drop-down list with predefined items splitted by two parts. Each item has an inner value for saving and a pair of displayed values. E.g. the collector will be able to see the same item but in different languages.

Properties:

* **Caption (left)**. Static text which will be placed above this element (at left).
* **Caption (right)**. Static text which will be placed above this element (at right).
* **Items**. A list of items.
* **Keep last value**. Whether to keep last entered value for this element during data collecting process.

Combobox
------

A drop-down list with predefined items which allows the selection of only one value.

Properties:

* **Items**. A list of items.
* **Keep last value**. Whether to keep last entered value for this element during data collecting process.
* **Own items**. User can add own items to this combobox.
* **Input with search**. Whether to show or not corresponding items during typing in this combobox.

Counter
-------

An element which automatically adds values based on some predefined format.

Properties:

* **Increment**. The value which is added to the current counter's value each time user collects data about an object.
* **Initial value**. Initial value from which incrementing starts.
* **Prefix**. A text which is added before the counter's value. If this text is not void the counter writes its value as a string.
* **Suffix**. A text which is added after the counter's value. If this text is not void the counter writes its value as a string.
* **Prefix from list**. Prefix from list.
* **Suffix from list**. Suffix from list.

Average counter
---------------

An element which counts an average value from some amount of entered values.

Properties:

* **Number of values**. How many values a collector can enter to count an average value.

Text edit
---------

An element for editing simple text or numbers.

Properties:

* **Initial text**. Initial text.
* **Keep last value**. Whether to keep last entered value for this element during data collecting process.
* **Max. lines count**. Maximum number of lines for this text edit.
* **NextGIS ID login**. The value in this text edit will be replaced with user's NextGIS ID login.
* **NextGIS Web login**. The value in this text edit will be replaced with user's login if the connection with NextGIS Web is established during the data collecting process.
* **Only numbers**. This element can accept only numbers.

Checkbox
------

An element which allows user to pick from two values: true or false.

Properties:

* **Initial value**. Initial value.
* **Keep last value**. Whether to keep last entered value for this element during data collecting process.
* **Text**. Displayed text

Photo
-----

An element which allows to take photos with embedded camera or to add them from the gallery.

Properties:

* **Max. photo count**. Maximum number of photos.
* **Comment**. Comment under photo(s).
