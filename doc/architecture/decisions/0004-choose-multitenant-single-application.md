# 4. Choose multitenant single application

Date: 2026-03-09

## Status

Accepted

Supercedes [1. Choose system components](0001-choose-system-components.md)

## Context

After chiecking with the people on charge of attendance control in this school I think is better to create a single app that can connect and use data from two database, one local an another one a server. This last server will be running local.

## Decision

We need to prepare the app to be able to connect and save/read/synchronize data from two different sources.

## Consequences

We will need to work really hard in creating an app that works on two differente modes and we need to be carefull on the synchronization feature.
