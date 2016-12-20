+++
date = "2016-12-20T14:13:10+11:00"
title = "RTP Media Server"
draft = false

+++

**(July 2013 - November 2013)**  
**Group Project**  
**Role: Lead Programmer, Presenter**

Written for the RMIT University module "Operating System Principles", this program acts as
a media server that supports simultaneous streams and users. Users can request movies by sending
a request to the server, which will respond with a movie stream to the client. This program
constructs the packets using the Real-time Transport Protocol (RTP) and sends them to the user via
the User Datagram Protocol (UDP).

### Functionality and features

*   Supports users watching the same stream.
*   Supports concurrent streams.
*   MPEG-1 files stored on the server, the packets created on the fly.
*   Designed to run on the Raspberry Pi, with low requirements.
*   Utilises multi-threading and processes.
*   Inter-process communication via pipes and shared memory.
*   Maintains concurrency integrity via semaphores.
*   Kernel module version available (as a proof of concept).