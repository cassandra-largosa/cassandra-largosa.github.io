---
layout: essay
type: essay
title: "Meteor Gotchas"
date: 2017-03-09
labels:
  - Software Engineering
  - Meteor
---

While working on my [digits](https://github.com/cassandra-largosa/digits) app there were a few issue with Meteor I ran into.

## Items missing in the database

When I added the Contacts Collection to digits the first time there had been items missing from the default database, only the first entry had appeared. While I was working adding the collection was that the app kept crashing while I fixed some variable names. Meteor tried to restart the app each time it crashed. During one of those restarts Meteor had successfully added the first entry from <code>contactsSeed</code> and since the seed was only supposed to be loaded when there was nothing else in the database even after adding all the entries. I had to quit the app and run <code>meteor reset</code> for all the entries to appear on the home page.