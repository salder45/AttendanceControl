# 1. Choose system components

Date: 2025-03-23

## Status

Accepted

## Context

This attendance software is made for a high school, this particular schools has different activities, that required register attendance, some of these activities are made on places with good Wi-Fi connection, some others don't have these good conditions. 
This situation make us to prioritize the robustness of the system and the capacity to work offline. Also is needed to consider that the system needs to be able to run in different devices.  

## Decision

This system is going to be composed by two parts each one with its own functions. 
1. Main System: Manage the creation of data for students, teachers, events. This one needs to run on a local machine with a database server running on it. Also allows to synchronize data from the attendance system.
2. Attendance System: Run for attendance taking, needs a local database, it can send attendance data with tne main system.

## Consequences

This make us to work on two systems and make us focus on make them able to synchronize the data (Generate an event, persons list/read data from the event)