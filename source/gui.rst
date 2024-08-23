.. sectionauthor:: Mikhail Gusev<mikhail.gusev@nextgis.ru>

.. _ngfb_gui:

User interface description 
=======================

The program looks like this by default: (:numref:`ngfb_gui_pic`).

.. figure:: _static/ngfb_gui_en.png
   :name: ngfb_gui_pic
   :align: center
   :width: 16cm

   Formbuilder's GUI

   Numbers show: 1 - main menu; 2 - main toolbar; 3 - “Updates available” icon; 4 - authorization button; 5 - "device" screen; 6 - “elements” menu; 7 - “Data” menu; 8 - “Properties” menu. 

You can change the position, size and visibility of the side menus:

   * Hover your mouse cursor over the menu and press the left button to transfer it to a different place;
   * Pull the menu’s edges to change its width and height;
   * Press the close button to hide menu. You can make it visible again in the main menu section “view”.

Main menu 
------------

The main menu consists of the following submenus:

**File**

    * **New**. Create a new blank project.
    * **Open**. Open project from .ngfp file.
    * **Save**. Save project to .ngfp file.
    * **Save as...**. Save project to another .ngfp file.
    * **Exit**. Exit application.

**Edit**

    * **Download from NextGIS**. Download form (and data) from your web GIS by selecting an existing layer.
    * **Upload to NextGIS**. Send a form to your web GIS with creating a new layer.
    * **Form properties**. Edit the main properties of the form: form’s name and geometry type of the layer.
    * **Clear form**. Delete all elements from the form. 
    * **Bind elements to fields**. Turn on/off the automatic field creation mode. While the mode is ON when new elements are placed on the form, fields of a layer are automatically created and attached to the elements. 

**View**

    * **Toolbars**. Hide/show different menus and interface panels.

**Settings**

    * **Language**. Choose interface language. Reload Formbuilder for changes to start working.

**Help**

    * **View help**. Open the help page in browser.
    * **Need commercial support?**. Open commercial support page in browser. 
    * **About**. Show About dialog. Also contains information about your account.

Main toolbar
--------------

Contains fast-access buttons to subsections of the main menu. Move the mouse over the button to see its name (in a popup message) and description (in the program’s status bar below).

.. note::
    Some toolbar buttons may be inaccessible, which is shown by a “lock” icon on the button. To get full access to all functions in the program: complete authorization, if subscribed you will gain access to a complete functionality. 

“Updates available” icon
-------------------------

A green square icon with an arrow (the top right corner by default) will be shown only if updates are available (Windows and Mac OS only). If icon is not shown, then there are no updates, or the program failed to connect to the update server. Click on icon to update the program: Formbuidler will close (with a suggestion to save the project if there are changes) and update dialog will open. Follow the steps of the installation wizard. After the dialog finishes working, the program will restart automatically.

Alternatively, you can run the NextGIS update wizard as a separate program from the NextGIS installation directory.

Authorization
-------------

The button with the avatar image (the top right corner by default) allows you to sign in with NextGIS services and get the extended functionality of the program if you have a subscription. Press the button, then in the pop-up window press “Sign in”. In the opened browser page enter login and password of your NextGIS ID, after that return to the program. Check that you have a “supported” account by clicking on the authorization button again. 

To log off press the authorization button once again and press “Sign out” in the pop-up window.

.. note::
    Authorization needs to be completed only once. The next time you start the program, you will sign in automatically. Please note that after launching the program it may take several seconds before the blocked functionality becomes available.

If you want to log into another account, sign out both in the program and in the browser.

On-premise Authorization
------------------------

If you want to login via the on-premise, you must specify the appropriate Endpoint in the authorization settings (Main menu -> Settings -> Authorization) (:numref:`Endpoint_Formbuilder_en`).

.. figure:: _static/Endpoint_Formbuilder_en.png
   :name: Endpoint_Formbuilder_en
   :align: center
   :width: 10cm

   Adding your own authorization server



Device screen
----------------

This is a screen layout of the real device on which data will be collected in NextGIS Mobile/Collector. It is designed to create a form: i.e. for placing, moving and grouping the elements of which the form consists and with the help of which the data about one object of the layer will be entered at the moment of data collection. elements in the form are arranged vertically, one after another. It is possible to group items by named tabs.

To *add* an element to the form - start dragging it with the cursor, while holding the left mouse button, from the “elements” menu (left by default) - the cursor will take the form of a squeezed hand. Alternatively, you can quickly add an element to the end of the form by clicking on it one time with the left mouse button, pressing the Ctrl key in the elements panel.

To *select* an element - click the left button on it once in the form. A red dotted frame will appear around the element.

To *move* an element - drag it by pressing the left button to any place on the form.

To *delete* an item, select it and press the Delete key on the keyboard. Deleting an item cannot be undone. Be aware of the fact that when you delete an element, the associated field(s) of the layer will also be deleted.

Form elements
---------------

This menu contains a list of all available elements that can be created on the form. Hover over an element to see tooltip with its description.

To *add an element* to a form drag it holding left mouse button onto the device screen in the middle (the pointer will look like a squeezed hand). Alternatively you can quickly add an element to the end of the form by left-click + Ctrl.

.. note::
    Some elements may be inaccessible, which is shown by a “lock” icon on the button. To get access to the full functionality, log in and make sure you have a corresponding subscription plan. 

"Data" menu
-------------

This menu contains a table of layer fields. In the Formbuilder program, only one form is edited in one project, tied to only one layer. Layer’s field(s) are created automatically when elements are added to a form. an element may have from 0 to 2 related fields. To see what elements are attached to what fields - select the element: if any fields are attached to the element, they will be highlighted in bold in the table.

When creating elements for fields, their name, alias and type are automatically generated:

    * **Name** cannot be changed;
    * **Alias** can be changed in the corresponding text string in the table. Type a new name in this line, the changes will be saved automatically;
    * **Type** can be changed in the corresponding drop-down list in the table. Select the required data type from the drop-down list - the changes will be saved automatically. Please note that the field type depends on the element itself and its properties (for example, the Date and Time element can save only “Date / Time” and “String” values ​​at the time of data collection, but cannot store an “Integer” value). For some elements, you can change their properties so that the corresponding data types become available (for example to allow a text field to inout only numeric values ​​— set the "Only numbers" property in the "Properties" menu table and change the data type of the field to "Integer" in the menu table "Data").


“Properties” menu
---------------

This menu contains the table of properties of the selected element. Select an element by clicking on it with the left mouse button. Change the properties in the table that appears - changes to the element will be saved automatically. Please note: a change in one property may entail a change in another property of this element due to their incompatibility or mutual influence on each other. Changing the properties of an element also leads to an increase or decrease in the number of available types for fields, associated with the element: you can track this in the “Data” menu table.
