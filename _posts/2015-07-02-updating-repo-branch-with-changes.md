---
layout: post
title:  "Updating a repo branch with changes from the master"
date:   2015-07-02
---

Here’s my step by step version of how to update a branch with changes from the master in terminal… 
(wanting to make sure I understand the steps!)

*EXAMPLE*
to merge changes from master to gh-pages (branch)

Push files to master:

* tiy-assignments git master 

	git add .
	git status
	git commit -m “”
	git push origin master
	git status

then:
	git checkout -b gh-pages
	(to create a new branch)

	or:
	git checkout gh-pages  
	(switches to already created branch)

* tiy-assignments git gh-pages

	git push origin gh-pages
	git add .
	git status
	git commit -m “”
	git push origin gh-pages

	git checkout master (switches to master)

* tiy-assignments git master  

	git merge gh-pages
	git push origin master
	git status (to verify)