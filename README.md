# weather
Unix command line utility to get weather forcasts from wunderground.com

Requires: libcurl, libjson

This is just a stupid little utility I wrote to go out and get the current weather forcast from wundeground.com
and display it on the command line.


Command examples:

$ weather

Returns a simple 1-line forcast for the current day

$ weather -a

Returns the forcast for all periods that wunderground.com returns in a single request (currently 4)

$ weather -#

Returns the forecast for the first # periods returned by wunderground.com (typically day and night, so -2 will get today and tonight)


Config file:  ~/weatherrc
File format:
key=nnn
city=sss
state=sss

The key is an API key that you must obtain from wunderground.com.  You can't have mine.  They're free.  Get your own.
The city and state are (obviously) the location you want the forecasts for



This is a quick-and-dirty utility I wrote as part of my robot project.  It's not terribly robust, and doesn't handle
errors particularly well.  It could use a lot of cleanup, but works well enough for my purposes, and I just thought I'd
throw it out there in case somebody else finds it useful.  Feel free to make use of it as you see fit, just don't blame
me if something goes horribly wrong and your cat goes outside and gets caught in the rain because my program returned the 
wrong forecast or something.



