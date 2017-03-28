********************
BORIS App user guide
********************


.. image:: logo_boris_500px.png
   :scale: 300%

**version 0.1**

BORIS web site: `www.boris.unito.it <http://www.boris.unito.it>`_

BORIS user guide: `boris.readthedocs.io <http://boris.readthedocs.io>`_


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


**BORIS App** lets the user code for live observations.

**BORIS App** is designed to be used with **BORIS** (Behavioral Observation Research Interactive Software).

**BORIS App** run on Android. You will have to install before the `Kivy Launcher <https://play.google.com/store/apps/details?id=org.kivy.pygame&hl=en>`_


Installation
============

1) Install the Kivy Launcher

BORIS App is developped in Python using `Kivy <https://kivy.org>`_ as user interface.
You must install the Kivy Launcher on your Android device before installing BORIS App.

https://play.google.com/store/apps/details?id=org.kivy.pygame&hl=en

You can run Kivy applications on Android, on any device with Android 2.2 +.


2) Install BORIS App on your Android device

Extract the ZIP archive on your computer and the extracted directory (boris_app) to /sdcard/kivy/.


/sdcard/kivy/boris_app





Use
===

1) Launch the BORIS App

* Start **Kivy Launcher** 

.. image:: kivy_launcher.png
   :scale: 50%

* Select BORIS App, you should see the following screen:

.. image:: home.png
   :scale: 50%

* Click on **Download project** button

.. image:: download_screen.png
   :scale: 50%

2) Transfer your project from BORIS Desktop to BORIS App user guide

* Launch **BORIS Desktop**

* Open the project containing the ethogram

* Start the project server (File > Project server)

.. image:: project_server.png
   :scale: 100%

* Check the "Download from BORIS" checkbox (default)

* Input the URL shown in BORIS Desktop (for example 192.168.1.2:33149) without spaces

* Click **Download project** button

You should receive the project from BORIS Desktop and obtain the following message:

.. image:: download_successfull.png
   :scale: 50%

The BORIS desktop should show you this message:

.. image:: project_sent.png
   :scale: 100%

3) Open the project

* Click the **Open project** button

* Select the new downloaded project

* Click the **Open project** button


4) Start a new observation

* Click the **New observation** button

.. image:: new_observation.png
   :scale: 50%
   
* Input an **Observation Id** (mandatory, this id must be unique in your project)

* Change the date (optional)

* Input a description for your observation (optional)

* If independent variables are defined, click on the **Independent var** button
and fill the value for each variable.

* Click the **Start observation** button


5) Stop the observation

* Click on the **Stop observation** red button. Confirm that you want to quit.

6) Sending observation to BORIS desktop

* Start the project Server on BORIS desktop (**File > Porject server**)

* On BORIS App, open the project containing the observation to send.

* Click the **Send observation** button

* Select the observation you want to send in the observations' list

* Input the URL of project server

.. image:: send_observation2.png
   :scale: 50%
