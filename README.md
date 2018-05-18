Region Östergötland's fork of the international openEHR.org CKM mirror, plus local templates and archetypes
===========================================================================================================
The intention of this "fork" is to make it simple to work with archetype and template tools to create local content based on international archetypes. You can download a zip (or maintain a GIT-clone/fork/link) of this repository in order to access the combination of international and local archetypes and templates in your tools. 

If you are using Marands online ADL-designer and nobody in your organization has yet atdded this repo, then this setting should work:
Repositories (top menu bar) --> New repository (button) -->

  Repository type: GitHub
  Repository name: RÖ fork of CKM-mirror (or whatever you want to call it)  
  Owner: regionostergotland
  Repository: openehr_definitions 
  Branch: master

Update policy
------------
We do occasional manual one-way updates from https://github.com/openEHR/CKM-mirror (that most often update the content of the '/local/archetypes' subdirectory tree). The direction is always _from_ the international CKM tool (automatically) to https://github.com/openEHR/CKM-mirror and from there (manually) to this fork https://github.com/regionostergotland/CKM-mirror/.

If we find an error or want to contribute new content to the international repository, then the web-based tools at http://ckm.openehr.org should be used for submitting such content. Files in this fork will _not_ be synced back automatically to the international repository.

Howto-instructions for RÖ-repo admins to update this repository to get the latest content from the international one: 
* With command-line tools https://help.github.com/articles/syncing-a-fork/ or
* Using the web: https://www.sitepoint.com/quick-tip-sync-your-fork-with-the-original-without-the-cli/

Directroy names and content
---------------------------
Warning: the directory names are a bit confusing due to conventions and tools used "upstream"

* `/local`  currently contains Region Östergötland's locally created archetypes and templates all in the same directory, no matter what openEHR class they are based on. (This seems to be the directory preference of some tools.)
* `/local/archetypes`, `/local/templates` and `/local/templates` contain directories copied straight from openEHR's international online CKM tool http://ckm.openehr.org via https://github.com/openEHR/CKM-mirror
* `/remote/` contains subdirectories like `no.nasjonalikt/archetypes` that have been copied from "national/regional" CKMs like http://arketyper.no/ckm/ into openEHR's international online CKM tool http://ckm.openehr.org they are thus "remote" with respect to the international CKM as opposed to the `/local/archetypes` considered local with respect to the international CKM. 

Thus, part of what is under `/local` is truly local to Region östergötland and part of it (e.g. `/local/archetypes`) comes from teh international space...

Future setup?
-------------
If this works fine and there is interest, then the chain could be modified to instead become openEHR --> SKL (or EHM?) --> Region Östergötland 

--------------

Original text from https://github.com/openEHR/CKM-mirror:

openEHR Foundation International CKM Mirror 
===========================================

This is a mirror of the not-for-profit international openEHR.org Clinical Knowledge Manager (CKM) clinical models repository at www.openehr.org/ckm

It contains archetypes, templates and termsets on the CKM Authoring TRUNK, and will include both published assets and unpublished/unstable assets undergong active development and review.

All of these assets are licenced under a Creative Commons Attribution-ShareAlike 3.0 licence ![CC-BY-SA License](https://i.creativecommons.org/l/by-sa/3.0/88x31.png) and can be used freely within open source or commercial applications.

This mirror auto-updates whenever the CKM TRUNK changes.

If you would like to contribute to development or review of the models, please register at www.openehr.org/ckm


