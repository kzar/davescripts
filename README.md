# Davescripts

## Introduction

Small shell / Python scripts I find useful.

## onceonline

Often when working on a train or somewhere else with intermittent internet
access I need to run a command once I'm back online. Constantly checking is a
distraction so I wrote this script. It will check every 5 seconds if the
computer is back online, if so it will run the given command.

Usage:

    ./onceonline COMMAND

## backup

Small script to make creating backups easier, avoids me needing to remember all
the arguments. Bastardized version of [this example](https://borgbackup.readthedocs.io/en/stable/quickstart.html#automating-backups).

