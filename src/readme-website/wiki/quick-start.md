# Quick Start

This video explains how to change a simple text element everywhere it appears.

<iframe width="560" height="315" src="https://www.youtube.com/embed/JDPPhjM1ods?si=MRtQuTsW98qgR5H4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

This video goes over, in depth, how a more complicated page is rendered.

TODO goal: understand how http://127.0.0.1:8000/authors/Author%20Who%20Asked%20To%20Be%20Credited%20Only%20As%20%E2%80%98He%20Who%20Shall%20Not%20Be%20Named%E2%80%99/ is rendered
  urlCONF https://docs.djangoproject.com/en/5.1/topics/http/urls/
    the view
      touch on class based views (link: https://docs.djangoproject.com/en/5.1/topics/class-based-views/) and why we don't use them
      models used in the view
      querying the models https://docs.djangoproject.com/en/5.1/topics/db/queries/
      render(), list the args
        request: taken care of by path(), probably 
        context: a mapping from a name to what that name refers to. come back to that later
        template_name: the html template. start explaining this