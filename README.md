# clean-stream-filters

This repository contains filters for editing movies for innapropriate content. These filters are designed to be used with the chrome extension [Clean Stream](https://chrome.google.com/webstore/detail/clean-stream/cppacmdbokpnibcconbcniibodcfgdba) but can be used freely by other filtering services.

## The .filter File Format

The .filter files are simple text files with the following layout:

```
title //this signifies that the title of the filter is on the following line
filter1 //this is the title of the filter
type //this signifies that the type of the filter is on the following line
0 //this is the type of filter1. The type can be either 0 (audio) or 1 (audio visual)
category //this signifies that the category of the filter is on the following line
test //this is the category of filter1
description //this signifies that the description of the filter is on the following line
This is a test filter.
startTime //this signifies that the startTime of the filter is on the following line
3 //this is the start time of filter1
endTime //this signifies that the endTime of the filter is on the following line
8 //this is the end time of filter1

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
```
