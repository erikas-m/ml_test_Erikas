Simple Github issues CRUD interface
========================

Welcome to the simple Github issues CRUD interface. This application allows you to use Github API v3 through the web interface.

This document contains information on how to use this application.

1) Demo
----------------------------------

To check out how this application works, check out demo version on */web route.

2) CRUD routes and usage
-------------------------------------

Issue creation:     */web/{owner}/{repo}/create
Issue retrieval:    */web/{owner}/{repo}/find       - search for issues dialog
                    */web/{owner}/{repo}/findAll    - lists all repository issues
                    */web/{owner}/{repo}/show/{num} - shows concrete issue
Issue update:       */web/{owner}/{repo}/edit/{num} - issue edition dialog

Issue deletion is not available on Github. Closing issues possible through update route.

{owner} -   Repository owners login
{repo}  -   Repository name
{num}   -   Issue number

3) Known issues
--------------------------------

In issue search, state selection doesn't work. Github API returns all issues, no matter which state is provided.
Error should be in Github API or KnpLabs php-github-api lib.

4) License
--------------------------------

All code can be used and modified without any restrictions.

5) To do list:
--------------------------------

Write tests.

6) Words from author
--------------------------------

This is my first symfony2 individual project. If there are any issues, please post it in repository.