## 2025-02-26 CAC-DC-Image Meeting

* Meeting connection information: [Zoom meeting](https://openmicroscopy-org.zoom.us/j/83692938188?pwd=Yzc4Yk5tOFYxbTVQcHpMODdDSU0yQT09)
* Date and time: [February 26, 2025, 18:00 UTC](https://www.timeanddate.com/worldclock/fixedtime.html?msg=CAC+Meeting+DC+Image+Processing&iso=20250226T18&p1=1440&ah=1)

### Sign-in

- Marianne Corvellec
- Josh Moore
- Erick Ratamero
- Ulf Schiller

### Agenda

* [GloBIAS in-person workshop](https://forum.image.sc/t/globias-and-data-carpentry-in-person-workshop-for-image-processing-in-python/108061)
    * Marianne is planning to attend (selection in process)
* OER (Open Educational Resources) survey by Gerit Wagner and Laureen Thurner (University of Bamberg)
  - survey designed to explore:
    - The nature and types of OER
    - Structures and processes for OER creation
    - Challenges and solutions in applying OER effectively
  - possible followup when results are publicized
* scikit-image update
    * v0.25 release, followed by two [patch](https://github.com/scikit-image/scikit-image/releases/tag/v0.25.1) [releases](https://github.com/scikit-image/scikit-image/releases/tag/v0.25.2)
        * watershed algorithm -> recent 'fix' had induced (very) different results -> conversation is still active, cf. https://github.com/scikit-image/scikit-image/issues/7709
        * blur metric -> when passing a uniform image, the result would be NaN, now, it's handled gracefully, so the metric equals 1 as 'expected' (i.e., fully blurry)
    * [typing our API](https://github.com/scikit-image/skimage-archive/tree/main/grants/2022_CZI_EOSS5)
        * [docstub](https://github.com/scientific-python/docstub)
    * [dispatching](https://github.com/scikit-image/scikit-image/pull/7520)
    * [to-do list](https://github.com/scikit-image/scikit-image/wiki/API-changes-for-skimage2#proposed-api-changes-surrounding-skimage2) for [skimage2 transition](https://discuss.scientific-python.org/t/yet-another-pathway-towards-skimage-v2)
        * skimage library may be come more like a protocol, separating the backend, currently experimenting with a dispatching mechanism for running various implementations/backends
        * short term: add a note/callout to point out possibility of using another backend
* Medical/MRI Image Processing
    * a lesson has been proposed for the incubator
    * will need to be taught in alpha or beta
* Date for next meeting: May 28, 2025
