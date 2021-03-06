====================
BORIS App user guide
====================

:Author: `Olivier Friard <http://www.di.unito.it/~friard>`_

.. image:: logo_boris_500px.png
   :scale: 300%

**version 0.2.2**

**Be careful! This version must be considered as an ALPHA version only for testing**

.. contents::
    :depth: 2
    :backlinks: none



Legal
=====

Copyright 2017 Olivier Friard - Marco Gamba

**BORIS App** is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2, or any later version.

**BORIS App** is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
`GNU General Public License <http://www.gnu.org/copyleft/gpl.html>`_ for more details.



Introduction
============


**BORIS App** is an event logging app for live observations.

**BORIS App** is designed to be used with **BORIS** (Behavioral Observation Research Interactive Software, v. 4+) and share with it the project format.

**BORIS App** run on Android (2.2+). You will have to install the `Kivy Launcher <https://play.google.com/store/apps/details?id=org.kivy.pygame&hl=en>`_




Installation
============

Install the Kivy Launcher
-------------------------

BORIS App is developped in Python using `Kivy <https://kivy.org>`_ as user interface.
You must install the Kivy Launcher on your Android device before installing BORIS App.

https://play.google.com/store/apps/details?id=org.kivy.pygame&hl=en

You can run Kivy applications on Android, on any device with Android 2.2 +.


Install BORIS App on your Android device
----------------------------------------

The BORIS App is available on the BORIS App GitHub repository: `https://github.com/olivierfriard/BORIS-App/releases <https://github.com/olivierfriard/BORIS-App/releases>`_




Extract the zip (or tar.gz) archive on your computer and copy the extracted directory (BORIS-App-VERSION) to :code:`/sdcard/kivy/`.

For example:

.. code::

 /sdcard/kivy/BORIS-App-VERSION




**If the /sdcard/kivy directory does not exist on your Android device you must create it**


Use
===

Launch the BORIS App
---------------------

* Start **Kivy Launcher**

.. image:: kivy_launcher.png
   :scale: 50%

* Select BORIS App, you should see the following screen:

.. image:: home.png
   :scale: 50%





Transfer your project from BORIS to BORIS App
---------------------------------------------

This operation requires an internet connexion.

* Launch **BORIS** on your desktop or laptop computer (see www.boris.unito.it). This version of BORIS App works only with the **v. 4+** of BORIS Desktop.

The BORIS user guide is available at `boris.readthedocs.io <http://boris.readthedocs.io>`_


* Open the project containing the ethogram you want to transfer to BORIS App

* Start the project server (File > Project server)

.. image:: project_server.png
   :scale: 100%


* On BORIS App press the **Download project** button

.. image:: download_screen.png
   :scale: 50%


* Check the "Download from BORIS" checkbox (default)

* Input the URL shown in BORIS on Desktop/Laptop computer (for example 192.168.1.2:33149) without spaces

* Press the **Download project** button

You should receive the project from BORIS Desktop and obtain the following message:

.. image:: download_successfull.png
   :scale: 50%

The BORIS desktop should show you this message:

.. image:: project_sent.png
   :scale: 100%






Open the project
-----------------

* Press the **Open project** button

* Select the new downloaded project

* Press the **Open project** button


BORIS App will show a summary of the selected project:

.. image:: project_details.png
   :scale: 50%


Start a new observation
-----------------------

* Press the **New observation** button


.. image:: new_observation.png
   :scale: 50%


* Input an **Observation id** (mandatory, this id must be unique in your project)

* Change the date (optional, default: current date time)

* Input a description for your observation (optional)

* If independent variables are defined, click on the **Independent var** button and fill the value for each variable.


.. image:: independent_variables.png
   :scale: 50%

* Press the **Start observation** button

You will obtain a screen with buttons corresponding to behaviors defined in your project.
You can press it to code behaviors. The event time will be recorded in your observation.



.. image:: running_observation_without_categories.png
   :scale: 50%



If behavioral categories are defined in your project, the behaviors will be grouped by category and
buttons will be colored.

.. image:: running_observation.png
   :scale: 50%




Select the focal subject
-------------------------

* Press the **Select focal subject** button

* Select the focal subject. If the focal subject is already selected, the subject will be deselected.

.. image:: select_focal_subject.png
   :scale: 50%

The focal subject will be show in the green button (at left bottom).

.. image:: running_observation_selected_subject.png
   :scale: 50%


State events
------------

If you press on a state event, the corresponding behavior button will be highlighted in red until you press it again
to stop the state event.

.. image:: state_event.png
   :scale: 50%




Modifiers selection
-------------------

If modifiers are defined for the triggered behavior, BORIS App will show the modifiers page.

They are 3 types of modifiers:

* Single item selection from a list

* Multiple items selection from a list

* Numerical

Various sets of modifiers can be defined for a behavior.

BORIS App will show a page with all sets of modifiers defined for the current behavior.

Example for one set of modifiers (single item).
...............................................

.. image:: select_modifiers_1set_single.png
    :scale: 50%


Example for one set of modifiers (multiple items). 2 modifiers are selected.
............................................................................


.. image:: select_modifiers_1set_multiple.png
    :scale: 50%


Example for 2 sets of modifiers (single item)
..............................................

.. image:: select_modifiers_2sets.png
    :scale: 50%




Stop the observation
---------------------

* Press the **Stop observation** red button. Confirm that you want to quit.

The observation will be saved in the current project.




Sending observation to BORIS
-----------------------------


You can send an observation back to BORIS running on your desktop/laptop computer (requires an internet connexion).

* Start the project Server on BORIS desktop (**File > Project server**)

* On BORIS App, open the project containing the observation to send.

* Press the **Send observation** button

* Select the observation you want to send in the observations' list


.. image:: send_observation1.png
   :scale: 50%


* Input the URL of project server

.. image:: send_observation2.png
   :scale: 50%

* Press the **Send observation** button

The observation will be added to the current project of BORIS desktop. If an observation with same id already exists
BORIS will ask you for renaming it or overwriting it.


Limitations
===========

These limitations should be fixed in next releases.


* BORIS App can not handle independent variables defined as **set of values**

