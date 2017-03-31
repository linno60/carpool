# Carpool Application
An application which link student drivers and passengers. The goal is to save time and make benefits.

## Motivation
Imagine A and B live close by, they go to same school and have similar class schedules. A goes to school by bus, which takes time, whereas B drives to school, which costs money. Why don’t they share the ride, and the costs together? In this way, they can both save time and money. 
The application will require users to login with facebook account, do the calculation based on each user’s daily routine, and find the best matching carpool partner.

## Getting Started

This README would normally document whatever steps are necessary to get the application up and running.

## Algorithm

We want something that would be flexible to changes, and not penalize anyone for not participating.  That is, what you get out is proportional to what you put in.

The gist of a suitable algorithm is as follows:

**Example:**

 * Alice = 0, Bob = 0, Carol = 0.  Anyone can drive; we'll pick Alice.
 * Alice = 8, Bob = -4, Carol = -4.  It's between Bob or Carol.  We pick Bob.
 * Alice = 4, Bob = 4, Carol = -8.  Carol's turn.
 * Alice = 0, Bob = 0, Carol = 0.  After the last ride, everyone is square.  We'll pick Alice because she drove least recently.

Now let's watch what happens when someone misses a day (continuing the previous example):

* Alice = 8, Carol = -4.  Bob's out for the day, so it's Carol's turn. (Note that balances move by 12 / 2 = 6 instead of 4 this time.)
* Alice = 2, Bob = -4, Carol = 2.  Now the scheduler picks Bob.
* Alice = -2, Bob = 4, Carol = -2.  Alice drives because Carol drove more recently.

We fall into a different rotation order, but continue to spread the load evenly.

## Setup

* Create users
* Create car pool(s)
 * Set which weekdays the car pool operates (default M-F)
 * Set exceptions (days the carpool does not operate, such as holidays)
 * Set overrides (days the carpool operates outside the normal weekly schedule)
 * Add users
* Set user schedules
 * Each user can click the calendar icon next to the carpool on the front
   page to set his or her own days of participation in the carpool (e.g.,
   excluding Tuesdays and an upcoming holiday trip)
   
   
## Limitations

Features I intend to add someday include:
* Email/SMS notifications
* Confirmation of rides, visible to others
* Transfering credits between drivers (e.g., "I'll buy you lunch if you take my turn tomorrow.")
* Some kind of permission structure (everyone is an admin currently)

## Development

Please feel free use a different markup language if you do not plan to run rake doc:app.

## Technical info

This is a Rails 3.2 bundler application.

## The MIT License (MIT)

Copyright (c) 2015

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

