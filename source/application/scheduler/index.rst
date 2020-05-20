.. _scheduler:

##############
Scheduler
##############

The scheduler allows to schedule the playlists to broadcast, and it takes care to update the
`playout <https://en.wikipedia.org/wiki/Playout>`__ every time there's a change from one playlist to the other.

To access the 'Scheduler', open the **PROGRAM** menu and click on **SCHEDULER**.

.. figure:: img/program-sub-nav-scheduler.png

.. _scheduler-overview:

*********
Overview
*********

The scheduler is composed of 3 elements:

* The calendar navigation menu (orange).
* The calendar (green).
* The playlists clipboard (blue).

.. figure:: img/scheduler-overview.png

.. _scheduler-nav-menu:

The navigation menu
===================

The navigation menu allows to customize the calendar view and the data displayed in it.

.. figure:: img/scheduler-nav-menu.png

The available options are:

* **< Week** / **Week >**: Move one week backward / forward.
* **< Day** / **Day >**: Move one day backward / forward.
* **-** / **+**: Decrease / increase the height of the time slots.
* **7 Days** / **14 Days** / **28 Days**: Change how many days to display.
* **Reset**: Reset settings to the default values.
* **15** / **30**: Change the grid steps from 15 to 30 minutes.
* **Colors**: Change the color of the playlist in the grid (it does not affect the playlists already scheduled).
* **FS**: Switch to full screen (click again to return to the default setting).


.. _scheduler-calendar:

The calendar
=============

.. figure:: img/scheduler-grid.png

The calendar is composed of the following elements:

* **X axis**: The name and number of the day (the current day is highlighted in red).
* **Y axis**: The dayparts (from 6 a.m. onwards)
* **Current time cursor**: The cursor displaying the current time / position on the grid (highlighted in red).
* **Grid**: The area to place the playlists to broadcast.

.. _scheduler-clipboard:

The playlists clipboard
=======================

The clipboard lists the playlists waiting to be scheduled.

To add a playlist to the clipboard, go the :ref:`playlists list <playlist-list>` page, click on the **more options**
menu of the playlist and select **Schedule for playout**.

.. figure:: img/playlist-schedule-for-playout.png

The playlist(s) will be automatically added to the clipboard.

.. figure:: img/scheduler-clipboard-with-playlist.png

To clear / empty the entire clipboard click on **Clear Clipboard**. To remove a specific playlist click on the
**delete** button within it.

.. _scheduler-schedule-playlist:

**********************
Scheduling a playlist
**********************

To schedule a playlist, drag it from the clipboard and drop it on any empty slot (playlists can't overlap).

.. figure:: img/scheduler-drag-playlist-to-grid.gif

.. _scheduler-unschedule-playlist:

************************
Unscheduling a playlist
************************

To unschedule a playlist, double click on the title of the playlist to open the emission panel and click on
**REMOVE EMISSION**

.. figure:: img/scheduler-remove-playlist-from-grid.png

Playlists placed in the slots preceding the current day and time cannot be removed.




