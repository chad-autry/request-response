### Status
[![Build Status](https://travis-ci.org/chad-autry/request-response.svg?branch=master)](https://travis-ci.org/chad-autry/request-response)

# request-response
Utility project to assist with multiple requests/responses across a read and write stream
Uses ASCII Group Separator to delimit messages, and a fixed width (4 character) requestId to match responses to a callback given with the originating request
Both 'client' and 'server' processes look and act the same. One side must declare to use even requestIds and the other odd.