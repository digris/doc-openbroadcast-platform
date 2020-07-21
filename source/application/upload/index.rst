.. _upload:

#######
Upload
#######

.. _upload-overview:

********
Overview
********

The upload module allows you to upload and import recordings (audio files) in the library.

To access it, open the **CONTENT** menu and click on **UPLOAD**.

.. figure:: img/main-nav-content-upload.png

Click on **ACCEPT TERMS & UPLOAD MUSIC** to confirm that you agree to our
`Terms & Conditions <https://www.openbroadcast.org/about/terms-and-conditions/>`__ and that you have read this
:ref:`documentation <upload>` and understand how importing works.

.. figure:: img/upload-how-to-accept-terms.png

.. figure:: img/upload-main-view-overview.png

The module is composed of 2 elements:

* The area where are listed the uploaded file(s) *(orange)*.
* The summary of the current upload session *(blue)*.

See also:

* :ref:`Uploading files <upload-new-upload-upload-file>`

.. _upload-media-info-card:

File info card
==============

While a file is uploaded, it is processed to extract the music information/metadata stored in it (i.e., ID3 container
for mp3 files or Vorbis for Flac files).

Besides, the system also generates an audio fingerprint for the file. The information will help to:

* Manage and discover duplicates in the library.
* Find matches on Musicbrainz, an open music encyclopedia that collects music metadata and makes it available to the
  public.

The 'info card' (blue) displays the information associated with each uploaded file.

.. figure:: img/upload-media-card-list.png

The card's appearance will vary depending on the processing result, below the most common one, which alerts that
mandatory information is missing.

.. figure:: img/upload-media-card-overview.png


It is composed of the following elements:

Header
------

The original filename and file extension (as displayed in the computer file browser).

.. figure:: img/upload-media-card-header.png

File metadata
-------------

The information found in the file's metadata container (as displayed on most audio players).

.. figure:: img/upload-media-card-metadata.png

Mandatory information
---------------------

The information you need to complete to continue import the file.

.. figure:: img/upload-media-card-mandatory-fields.png

Actions
-------

The actions you can take on the file, which are:

.. figure:: img/upload-media-card-footer-functions.png

* **Remove file**: Remove and don't import the file.
* **Scan again**: Create an audio fingerprint and search matches on Musicbrainz (`acoustic ID <https://acoustid.org/>`_).
* **Continue import**: Import the file.

See also:

* :ref:`Reviewing the files information <upload-new-upload-review-file>`

.. _upload-summary-current-import:

Summary panel
=============

The state of the current upload session automatically updates whenever the information is completed, or an action is
taken on the file(s).

.. figure:: img/upload-summary-upload-session.png
   :width: 320px
   :height: 425px

The summary includes:

* **Ready to import:** The file(s) ready to be imported in the library.
* **Import completed:** The file(s) imported in the library.
* **Duplicates:** The file(s) recognized as :ref:`a possible duplicate <review-possible-duplicate>`.
* **Processing:** The file(s) has been processed (placed in the import queue).
* **Information needed:** The file(s) missing :ref:`mandatory information <review-mandatory-information>`.
* **Errors:** The errors occurred uploading / importing file(s).

.. _upload-how-to:

*******
How-tos
*******

.. _upload-new-upload-upload-file:

Uploading files
===============

To start a new upload session, open the **CONTENT** menu, and click on **UPLOAD**.

.. figure:: img/main-nav-content-upload.png

Click on **ACCEPT TERMS & UPLOAD MUSIC** to confirm that you agree to our
`Terms & Conditions <https://www.openbroadcast.org/about/terms-and-conditions/>`__ and that you have read this
:ref:`documentation <upload>` and understand how importing works.

.. figure:: img/upload-how-to-accept-terms.png

Click on **ADD FILES** to open the computer file browser and select the files or drag-n-drop them into the white frame.

.. warning::

   Currently supported audio formats are mp3, m4a, wav, ogg and flac.

.. figure:: img/upload-how-to-add-files.png

Upload will starts automatically.

.. _upload-new-upload-review-file:

Reviewing the files information
===============================

The appearance of the file 'info card' will vary depending on the processing result, below the most common cases:

* Mandatory information is missing.

  .. figure:: img/upload-media-card-how-to-review-mandatory-information.png

     Read more about in the section: :ref:`Completing mandatory information <review-mandatory-information>`.

* The system recognized the file as a duplicate (it may already exist in the library).

  .. figure:: img/upload-media-card-how-to-review-possible-duplicate.png

     Read more about in the section: :ref:`Managing duplicate files <review-possible-duplicate>`.

* The audio fingerprint of the file matches with a recording on `Musicbrainz <https://musicbrainz.org/>`_.

  .. figure:: img/upload-media-card-how-to-review-match-on-musicbrainz.png

     Read more about in the section: :ref:`Selecting a match on Musicbrainz <review-match-on-musicbrainz>`.

* The file has been automatically imported into the library because it was pre-tagged with `Picard <https://picard.musicbrainz.org/>`_.

  .. figure:: img/upload-media-card-how-to-review-pre-tagged-file.png

     Read more about in the section: :ref:`Files pre-tagged using Picard <review-pre-tagged-file>`.

.. _review-mandatory-information:

Completing mandatory fields
===========================

Mandatory information is used by the system to import and organize the recording in the library.

.. figure:: img/upload-media-card-how-to-review-mandatory-information.png

The information is:

* **Title:** The title of the recording.
* **Release:** The title of the release the recording appears on.
* **Artist:** The name of the artist(s) the recording is primarily credited.

The fields can be completed manually, by typing in it, or automatically, populating them with the file metadata
(read more about in the section: :ref:`Filling mandatory fields with metadata <complete-mandatory-with-metadata>`).

.. note::

   You can add more information later using the specific :ref:`release <release-form>`, :ref:`artist <artist-form>`,
   :ref:`track <track-form>`, or :ref:`label <label-form>`  forms (i.e., cover art, record label, additional artists, etc.).

.. _complete-mandatory-manually:

Completing information manually
-------------------------------

Click on the field and start typing in it. Once finished, click outside the field to confirm the entry.

.. figure:: img/upload-media-card-how-to-complete-title-field.gif

Note that typing inside the 'Release' or 'Artist' fields activate the auto-completion, listing all profiles in the
library whose name matches the current text typed in.

.. figure:: img/upload-media-card-release-field-auto-completion.png

This feature helps you to check if a release or artist associated with the recording is already available in the library.

The following examples show how to create a new release (not available in the library) and how to assign an artist that
is already in the library. The procedures are interchangeable.

.. _create-release-for-media:

**Creating a new release profile**

When the auto-completion opens up, click outside the list to close it.

.. figure:: img/upload-media-card-how-to-create-release.gif

The alert **+ Create** informs that it will create a new release profile.

If the recordings in the current upload session are part of the same release (i.e., an entire album), type the 'Release'
title only in one card and click on **Apply to all** to complete the field on the other cards at one go.

.. figure:: img/upload-media-card-how-to-apply-release-to-all.png

.. warning::

   We are aware of a bug where the system assigns the recording to the existing releases without letting you create
   a new profile. To get around the problem, check the box 'Force creation.'

   .. figure:: img/upload-media-card-how-to-force-creation-01.png

   Note the alert switches from **Assigned** (wrong) to **+ Create** (correct).

   .. figure:: img/upload-media-card-how-to-force-creation-02.png

      **'X' matches** only informs that an 'X' number of releases with the same title are available in the library.


.. _assign-artist-to-media:

**Assigning an artist profile**

When the auto-completion opens up, click on the matching artist to select it.

.. figure:: img/upload-media-card-how-to-assign-artist.gif

The alert **Assigned** confirms the assignment. Move the cursor over it to display the artist's information.

If the recordings in the current upload session are credited to the same artist (i.e., an entire album by artist 'X'),
type the 'Artist' name only in one card and click on **Apply to all** to complete the field on the other cards at one go.

.. figure:: img/upload-media-card-how-to-apply-artist-to-all.png


See also:

* :ref:`Importing files in the library<upload-import-file>`


.. _complete-mandatory-with-metadata:

Completing information using metadata
-------------------------------------

Click anywhere on the 'File metadata' element to transfer the information to the respective mandatory fields.

.. figure:: img/upload-media-card-how-to-select-metadata.png

    The green checkmark confirms the transfer was successful.

While transferring the information, the system will check if an artist or release with the same name is already in the
library and assign it. Verify the accuracy of the assignments and correct where needed.

See also:

* :ref:`Creating a new release profile <create-release-for-media>`
* :ref:`Assigning an artist in the library <assign-artist-to-media>`
* :ref:`Importing files in the library<upload-import-file>`


.. _review-match-on-musicbrainz:

Choosing a match on MusicBrainz
===============================

'Possible releases' lists all recordings found on MusicBrainz matching with the audio fingerprint generated for the file
(`Acoustic ID <https://acoustid.org/>`_).

Click on a match to transfer the information.

.. figure:: img/upload-media-card-how-to-select-match-on-musicbrainz.png

    A green checkmark will highlight the chosen match.

See also:

* :ref:`Importing files in the library<upload-import-file>`


.. _review-possible-duplicate:

Managing a possible duplicate
=============================

'Possible duplicate' indicates the recording may already exist in the library.

.. figure:: img/upload-media-card-how-to-review-possible-duplicate.png

The options are:

#. Click on **REMOVE FILE** to remove and don't import the file.
#. Click on **RE-IMPORT FILE** to ignore the warning (i.e., false positive).

After clicking on **RE-IMPORT FILE**, you may need to :ref:`review the mandatory information <review-mandatory-information>`.

.. hint::

  To verify the detection's accuracy, right-click on the title of the 'possible match' and select 'open in a new tab.'
  Check the duration or listen to the audio file to ensure it was not a 'False Positive' case.

.. _review-pre-tagged-file:

Pre-tagged file
---------------

File(s) previously tagged using the Picard tag editor are automatically imported in the library (no additional steps required).

.. figure:: img/upload-media-card-how-to-review-pre-tagged-file.png

`Picard <https://picard.musicbrainz.org/>`__ is a desktop music tagger by `Musicbrainz <https://musicbrainz.org/>`__,
which insert identifiers
(`Musicbrainz ID <https://musicbrainz.org/doc/MusicBrainz_Identifier>`__) in the file's metadata container.

.. figure:: img/mbrainz-picard-tag-editor.png

The system uses these identifiers to find matches and keep organized the recordings in the library.

.. _upload-import-file:

Importing files
===============

To import a file in the library, click on the **CONTINUE IMPORT** button within the file info card.

.. figure:: img/upload-media-card-footer-functions.png

The file will be added to the import queue (highlighted in blue) and then automatically imported.

.. figure:: img/upload-media-card-how-to-import-file.png

  The green color confirms the import was successful.

.. warning::

  We are aware of a bug where clicking multiple times on **CONTINUE IMPORT** will import numerous copies of the recording.
  To get around the problem, simply wait for a little after clicking it the first time. Click again on it only when you
  are sure the recording is not getting imported.

At this point you can:

* Click on the title to visit the :ref:`track profile <track-detail>` in the library.
* Click on the artist's name to visit the :ref:`artist profile <artist-detail>` in the library.
* Click on the release title to visit the :ref:`release profile <release-detail>` in the library.
* Continue to complete the information on the remaining files in the current upload session.

.. hint::

   Review each file's information and then click on **Import all** to import all files at one go.

   .. figure:: img/upload-how-to-import-all.png

