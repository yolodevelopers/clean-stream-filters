# clean-stream-filters

This repository contains filters for editing movies for innapropriate content. These filters are designed to be used with the chrome extension Clean Stream but can be used freely by other filtering services.

## The .filter File Format

The .filter files are simple text files with the following layout:

title //this signifies that the title of the filter is on the following line
filter1 //this is the title of the filter
type //this signifies that the type of the filter is on the following line
0 //this is the type of the filter. The type can be either 0 (audio) or 1 (audio visual)
category //this signifies that the category of the filter is on the following line
test //
description //this signifies that the description of the filter is on the following line
This is a test filter.
startTime //this signifies that the startTime of the filter is on the following line
3
endTime //this signifies that the endTime of the filter is on the following line
8

title //the above space signifies that the filter is ended and the next filter has begun
filter2
type
1
category
test
description
This is a test filter.
startTime
10
endTime
15

