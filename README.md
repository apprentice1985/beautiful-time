# BeautifulTime

[![travis-ci](https://travis-ci.org/restran/beautiful-time.svg?branch=master)](https://travis-ci.org/restran/beautiful-time)
[![Coverage Status](https://coveralls.io/repos/github/restran/beautiful-time/badge.svg?branch=master)](https://coveralls.io/github/restran/beautiful-time?branch=master)

BeautifulTime is a python package for convert date string, datetime, time and timestamp.

## Install

```
pip install BeautifulTime
```

## Usage

```py
import BeautifulTime

date_str = '2016-10-30 12:30:30'
dt = BeautifulTime.str2datetime(date_str)
# with a custom format
dt = BeautifulTime.str2datetime(date_str, format='%Y-%m-%d %H:%M:%S')
t = BeautifulTime.str2time(date_str)
ts = BeautifulTime.str2timestamp(date_str)

dt = BeautifulTime.str2datetime(date_str)
t = BeautifulTime.str2time(date_str)
ts = BeautifulTime.str2timestamp(date_str)

s = BeautifulTime.datetime2str(dt)
t = BeautifulTime.datetime2time(dt)
ts = BeautifulTime.datetime2timestamp(dt)

s = BeautifulTime.time2str(t)
dt = BeautifulTime.time2datetime(t)
ts = BeautifulTime.time2timestamp(t)

dt = BeautifulTime.timestamp2datetime(ts)
t = BeautifulTime.timestamp2time(ts)
s = BeautifulTime.timestamp2str(ts)
```
