## 2024-11-27 CAC-DC-Image Meeting

* Meeting connection information: [Zoom meeting](https://openmicroscopy-org.zoom.us/j/83692938188?pwd=Yzc4Yk5tOFYxbTVQcHpMODdDSU0yQT09)
* Date and time: [November 27, 2024, 20:00 UTC](https://www.timeanddate.com/worldclock/fixedtime.html?msg=CAC+Meeting+DC+Image+Processing&iso=20241127T20&p1=1440&ah=1)

### Sign-in

* Toby Hodges
* Josh Moore
* Ulf Schiller
* Erick Ratamero
* Marianne Corvellec

### Agenda

* Review [PR 328](https://github.com/datacarpentry/image-processing/pull/328): New animation to illustrate blurring
    * related issue observed that the current example of the eye of a cat did note clearly illustrate the effect of blurring. This PR uses a simplere, black-and-white example.
    * Erick: I like the new image
    * Toby: Me too, bigger question is where to store the source code?
        * two options: put it in `episodes/fig/source/` or create a public gist with the code and put the environment.yml info in the docstring
        * Erick: if the gist disappeared, would it materially change the lesson?
        * Toby: only in terms of maintainability
        * *Some back and forth, which led to a (lazy) consensus that we should go with the `episodes/fig/source` option* 

* Cheat sheet should be an editable file (question for maintainers?).
    * Toby: I was able to open the cheatsheet PDF in Inkscape and save as an SVG. Seemed to work ok…

* Medical Image Processing in Incubator: https://carpentries-incubator.github.io/medical-image-processing/
    * is the committee interested in adopting a curriculum on medical image processing in the future?
    * Ulf: keep an eye on it, and consider it again in the future based on how it develops?
    * Erick: agree. it fits with this idea we had in the past about offshoot lessons.
    * Toby: I think Candace would appreciate a response, even if it is "thanks for sharing, but not right now"


* GloBIAS and Data Carpentry bioimage analysis curriculum development meeting

> Dear colleagues,
> 
> Are you interested in working with the growing community of Bio-Image Analysts? As a part of the growing GloBIAS community, we have partnered with Data Carpentry to adapt, enhance and expand the current Data Carpentries Image Processing with Python curriculum. Our goal is to create a potential go-to course for beginner/intermediate-level students and researchers. This idea was developed within the community and aims at improving the availability of standardized bioimage analysis training material.
> 
> We are reaching out to you because of your expertise as well as your past interest in outreach and education in the field. Our aim is to organize an in-person meeting to discuss how to best approach this task (we do have some initial ideas already that we can share with you via GIT hub upon request) and start working on the concepts for the new course together; we aim to continue this in an asynchronous manner afterwards.
> 
> We are happy to share that our institute, ISTA, would be willing to host such a community in-person event, that is currently planned for April 7th and 8th 2025 in Klosterneuburg (near Vienna), Austria. We would be excited if you were able to join us during this event.
> 
> In order to bring this event to life and secure its funding, we would need a tentative confirmation of interest for participation from your side. We believe we can make a significant impact in the community, but we cannot achieve this without some initial (though non-binding) commitment from participants. We therefore kindly ask you to send us a short expression of interest in case you consider joining us, by replying to this email.
> 
> In case you would not be able to participate, however think you know someone who might, we would appreciate your recommendations. If you have any questions or need further clarification, please do not hesitate to reach out.

    * Josh: they are trying to keep it small, haven't heard back yet how many people have indicated interest
    * Toby has expressed strong interest but need support to fund travel+accomm

* look into other existing efforts to create materials related to image processing (e.g., subject specific materials) and discuss opportunities to synergize/centralize efforts
    * Erick: GloBIAS are a good community to stay in touch with on this.
    * Josh: need to balance community effort to develop curriculum, against quality and approach 
    * Toby: (and capacity of this committee to review it all!) Potentially an AI lesson program in the works, and I would like to see a crossover between the two projects if so, ML for image processing.
    * Erick: we already have this: https://thejacksonlaboratory.github.io/deeplearning-image-analysis-workshop/
    * Ulf: I complemented the lesson with a session on cNNs and received very positive feedback. Reluctant to develop anything about AI with Python, as APIs and tooling is changing very quickly.
    * Marianne: a lot of the rest of the scikit-image community are unaware of DC efforts. Keeping focus on bioimaging, as most likely source of funding. So new curriculum/sub-curricula on bioimaging would be of great interest. Also important to be aware that scikit-image v2 will be the new normal next year, so changes to lesson coming. (v2 will *not* be backwards compatible; v1 will still work but migration to v2 is the recommended approach.) Lesson could be a good playground to find out about impacts of changes to the API.
