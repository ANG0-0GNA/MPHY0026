.. _CalibrationBasedRegistration:

Calibration-Based Registration
==============================

Learning Objectives
-------------------


Methods
-------

Typically, methods in IGS, are sub-divided (e.g. in :ref:`bookPeters`) into:

* Manual
* Point-based
* Surface-based (also called Shape-based)
* Volume-based
* Calibration-based


Manual Registration
^^^^^^^^^^^^^^^^^^^

Use a mouse or gesture device to manually rotate/translate/scale a pre-operative CT dataset
so that it aligns with the intra-operative scene, e.g. live video.

* To get a feel for this `try manipulating this model, provided on-line by Kitware <https://kitware.github.io/vtk-js/examples/VolumeContour.html>`_.
* To overlay a 3D liver CT model over a 2D video image, giving an augmented reality feel, try:

.. code-block:: language

    python mphy0026_manual_registration.py \
    -b doc/registration/liver_background.png \
    -m doc/registration/liver.vtp \
    -c doc/registration/liver_camera.txt

in the root of the MPHY0026 (i.e. this course) git repo.

* *To Do*: record video of SmartLiver on LiverPhantom

Pros:

  * Easy to implement for rigid/scaling
  * Robust (no algorithm to fail)
  * Easy to validate, and get approved

Cons:

  * Hard to implement for non-rigid cases
  * Normally inaccurate
  * Time consuming
  * Highly user dependent
  * How to interact with the device? who? is the user sterile?
  * Hard to re-register, due to time and user variability for instance

Examples: [Pratt2012]_ [Thompson2013a]_

Point-Based Registration
^^^^^^^^^^^^^^^^^^^^^^^^

* Arun, Horn
* Fiducial marker types
* Typical accuracy?
* Systems?

Exercise
* Pelvis Phantom
* LEGO example
* Matt, MRI example

Surface-Based Registration
^^^^^^^^^^^^^^^^^^^^^^^^^^

* ICP
* ICP variants
* Typical accuracy?


Exercise
* Matt, MRI example, drag pointer
* SmartLiver example

Volume-Based Registration
^^^^^^^^^^^^^^^^^^^^^^^^^


Calibration-Based Registration
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Intra-op CT, Lap video, a la Nassir, Feuerstein
* Intra-op US, Lap video, a la Washington








