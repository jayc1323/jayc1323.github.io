---
title: Building a RPC Generator
date: 2025-12-03 14:00:00 -0400
categories: [System design,Computer Science]
tags: [project]  # keep lowercase
description: Building a RPC Generator
layout: post
---
# What is RPC ?
- RPC stands for Remote Procedure Calls , enabling a programmer/client to make function 
  calls on another machine/server as if it were made locally.
## What is the benefit ?
- Eliminates the programming overhead for a client , in terms of serializing function arguments and other 
  details that are usually associated with REST and takes lesser time compared to REST as data sent over 
  the network can be binary and incurs lesser overhead than common formats like JSON when sending data types like arrays/structs.
### Challenge : Building a code generator that generates client and server side stubs when given a interface definition file.
- An RPC Generator takes in a interface definition file with types and function definitions and generates 
  client and server side stubs to handle serialization and deserialization of arguments and other function call related data.

