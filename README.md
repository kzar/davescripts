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

## shittycal

Small script to download an .ics file from a server which doesn't provide stable
UIDs for events. The first time it's called it will simply download the file.
Each time after that it will compare the existing file with the new one, and
attempt to only patch relevant differences.

Limitations:

 - Very simplistic so far, only checks if a hunk contains DESCRIPTION.
 - Vulnerable to this [patch runs ed...](http://rachelbythebay.com/w/2018/04/05/bangpatch/) exploit.

Usage:

    ./shittycal calendar-url calendar-file.ics
