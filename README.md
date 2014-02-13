ClarionLiveAddin
================

IDE Pad with a countdown to the next ClarionLive webinar!

Binary version hosted here: http://clarionaddins.com/addins/ClarionLiveAddin.html

What is this?!
--------------

Just a fun project to see if it was possible to create an addin for the Clarion IDE using Clarion.NET. Turns out it is!!
It attempts to give you a countdown to the next [ClarionLive](http://www.clarionlive.com/ClarionLive) webinar.

How to Build
------------

* Install Clarion.NET by SoftVelocity
* Clone/Fork/Whatever this repo to get the source
* Open the ClarionLiveAddin.sln in Clarion.NET
* Edit the "Reference Path" in the ClarionLiveAddin project to point to the BIN folder of your Clarion 7/8/9 installation.
* Build the solution!

A word about the Reference Path
-------------------------------

As mentioned above, in order to build this project you need to adjust the reference path to match your local environment.
This is to ensure that the IDE can find the two "ICSharp" dlls that are referenced in the project. I am not sure of a better way to do this yet, if you have any ideas please let me know!

To get to the reference path property do this:
* Right-click on the ClarionLiveAddin project in the solution explorer and select Properties from the context menu.
* Go to the Reference Paths TAB and make your adjustments.

How to use the compiled assembly
--------------------------------

Take the files from the \Bin\Release or \Bin\Debug directory and place them in a subdir in one of the addin paths of the IDE you want to use this in. e.g. \Clarion9\accessory\addins\ClarionLiveAddin
Then when you start the IDE you should be able to find a new menu item called "ClarionLive Countdown" in the View menu!

