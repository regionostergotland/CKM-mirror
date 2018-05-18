Region Östergötland's fork of the international openEHR.org CKM mirror, plus local templates and archetypes
===========================================================================================================
The intention of this "fork" is to make it simple to work with archetype and template tools to create local content based on international archetypes. You can download a zip (or maintain a GIT-clone/fork/link) of this repository in order to access the combination of international and local archetypes and templates in your tools. 

Directory names and content
---------------------------
Warning: the directory names are a bit confusing due to conventions and tools used "upstream"

* `/local`  currently contains Region Östergötland's locally created archetypes and templates all in the same directory, no matter what openEHR class they are based on. (This seems to be the default directory for saving new files created in ADL-designer)
* `/local/archetypes`, `/local/templates` and `/local/templates` contain directories copied straight from openEHR's international online CKM tool http://ckm.openehr.org via https://github.com/openEHR/CKM-mirror
* `/local/regionostergotland/` a manually created subdirectory intended for (regularly) organizing Region Östergötland's files. Note that the tools do not save here by default. Further project/topic-specific subdirectories could be created, e.g. `/local/regionostergotland/surgery` - the subdirectories under `/local` seem to be read by several tools.
* `/remote/` contains subdirectories like `no.nasjonalikt/archetypes` that have been copied from "national/regional" CKMs like http://arketyper.no/ckm/ into openEHR's international online CKM tool http://ckm.openehr.org they are thus "remote" with respect to the international CKM as opposed to the `/local/archetypes` considered local with respect to the international CKM. 
* `/` The root directory, containing this readme file end som others cloned from the ckm-mirror. (It also seems to be where ADL-designer stores archetyper that you "import" (rather than create) using the tool.

Thus, part of what is under `/local` and it's subdirectories is truly local to Region östergötland and other parts of it (e.g. `/local/archetypes`) comes from the international space...

Tools, tool settings and behavoiurs
-------------
List of available modelling tools: https://www.openehr.org/downloads/modellingtools

### Marand's online ADL-designer
Please note the somewhat odd directory choices used for saving new anbd imported assets described above. Template files created in the tool are by default saved with a ".t.json"-file ending. They can also be exported to several formats.

If you are using Marand's online ADL-designer https://ehrscape.marand.si/designerv2 and nobody in your organization has yet added this repo, then this setting should work:

Repositories (top menu bar) --> New repository (button) --> Repository type: GitHub
```
  Repository name: RÖ fork of CKM-mirror (or whatever you want to call it)  
  Owner: regionostergotland
  Repository: openehr_definitions 
  Branch: master
```

### Local-file-based tools
If you are using Ocean's Template designer or other local-file-based tools it should be possible to either 
* download and unpack the zip-file of this repository, found under the green "Clone or download" button on the https://github.com/regionostergotland/CKM-mirror page or
* set up GIT client to keep in sync (this has a bit of learning curve...)

Update policy & instructions
----------------------------
We do occasional manual one-way updates from https://github.com/openEHR/CKM-mirror (that most often update the content of the '/local/archetypes' subdirectory tree). The direction is always _from_ the international CKM tool (automatically) to https://github.com/openEHR/CKM-mirror and from there (manually) to this fork https://github.com/regionostergotland/CKM-mirror/.

If we find an error or want to contribute new content to the international repository, then the web-based tools at http://ckm.openehr.org should be used for submitting such content. Files in this fork will _not_ be synced back automatically to the international repository.

Howto-instructions for RÖ-repo admins to update this repository to get the latest content from the international one: 
* With command-line tools https://help.github.com/articles/syncing-a-fork/ or
* Using the web: https://www.sitepoint.com/quick-tip-sync-your-fork-with-the-original-without-the-cli/

Howto-instructions for RÖ-repo admins regarding how to move a file uding GitHub's web tools: https://help.github.com/articles/moving-a-file-to-a-new-location/

Future setup?
-------------
If this works fine and there is interest, then the chain could be modified to instead become openEHR --> SKL (or EHM?) --> Region Östergötland 

We'd likely want to have separate directories for different templates. 

--------------

Original text from https://github.com/openEHR/CKM-mirror:

openEHR Foundation International CKM Mirror 
===========================================

This is a mirror of the not-for-profit international openEHR.org Clinical Knowledge Manager (CKM) clinical models repository at www.openehr.org/ckm

It contains archetypes, templates and termsets on the CKM Authoring TRUNK, and will include both published assets and unpublished/unstable assets undergong active development and review.

All of these assets are licenced under a Creative Commons Attribution-ShareAlike 3.0 licence ![CC-BY-SA License](https://i.creativecommons.org/l/by-sa/3.0/88x31.png) and can be used freely within open source or commercial applications.

This mirror auto-updates whenever the CKM TRUNK changes.

If you would like to contribute to development or review of the models, please register at www.openehr.org/ckm


