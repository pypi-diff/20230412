# Comparing `tmp/astronomica-0.0.6.tar.gz` & `tmp/astronomica-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astronomica-0.0.6.tar", last modified: Tue Apr 11 18:49:13 2023, max compression
+gzip compressed data, was "astronomica-0.0.7.tar", last modified: Wed Apr 12 01:45:40 2023, max compression
```

## Comparing `astronomica-0.0.6.tar` & `astronomica-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:13.095418 astronomica-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 18:49:03.000000 astronomica-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-04-11 18:49:13.095418 astronomica-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-04-11 18:49:03.000000 astronomica-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:13.095418 astronomica-0.0.6/astronomica/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-11 18:49:03.000000 astronomica-0.0.6/astronomica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-04-11 18:49:03.000000 astronomica-0.0.6/astronomica/astronomica.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-11 18:49:03.000000 astronomica-0.0.6/astronomica/libconversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-11 18:49:03.000000 astronomica-0.0.6/astronomica/suntiming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:13.095418 astronomica-0.0.6/astronomica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-04-11 18:49:13.000000 astronomica-0.0.6/astronomica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-11 18:49:13.000000 astronomica-0.0.6/astronomica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:49:13.000000 astronomica-0.0.6/astronomica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 18:49:13.000000 astronomica-0.0.6/astronomica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 18:49:13.000000 astronomica-0.0.6/astronomica.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:49:13.095418 astronomica-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-11 18:49:03.000000 astronomica-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:45:40.078642 astronomica-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-12 01:45:30.000000 astronomica-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-04-12 01:45:40.078642 astronomica-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-04-12 01:45:30.000000 astronomica-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:45:40.078642 astronomica-0.0.7/astronomica/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-12 01:45:30.000000 astronomica-0.0.7/astronomica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-04-12 01:45:30.000000 astronomica-0.0.7/astronomica/astronomica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-12 01:45:30.000000 astronomica-0.0.7/astronomica/libconversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-12 01:45:30.000000 astronomica-0.0.7/astronomica/suntiming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:45:40.078642 astronomica-0.0.7/astronomica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-04-12 01:45:40.000000 astronomica-0.0.7/astronomica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-12 01:45:40.000000 astronomica-0.0.7/astronomica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:45:40.000000 astronomica-0.0.7/astronomica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-12 01:45:40.000000 astronomica-0.0.7/astronomica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 01:45:40.000000 astronomica-0.0.7/astronomica.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 01:45:40.078642 astronomica-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-12 01:45:30.000000 astronomica-0.0.7/setup.py
```

### Comparing `astronomica-0.0.6/LICENSE` & `astronomica-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.6/PKG-INFO` & `astronomica-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 Metadata-Version: 2.1
 Name: astronomica
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates
 Home-page: https://github.com/PyndyalaCoder/astronomica
 Author: Siddhu Pendyala
 Author-email: elcientifico.pendyala@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/PyndyalaCoder/astronomica/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # astronomica
 
 ## Introduction and Purpose
+
 <b>Astronomica</b> is a simple python library based on formulas pioneered at https://www.aa.quae.nl/en/reken/zonpositie.html, and https://astronomica.w3spaces.com/. Scroll below to check out the documentation. This library does not depend on Astropy or Skyfield, but requires their installation for conversion purposes - some of our functions include interoperability of libraries - skyfield units to astropy units, etc.
 
 ### Note of Usage:
 <b>Astronomica is 100% free</b>!! It is also <b>driven by the <i>community</i></b>, so we welcome tips, bug fixes, and more methods added by users and the general python & astronomy community. You can also join our reddit community at https://www.reddit.com/r/pythonlibraries/ 
 
 
 ## Usage:
 Here is a very simple usage example of Astronomica:
 
 ```python
-
 from astronomica import *
-
 lunar_phase = getLunarPhase()
 planting_time = False
 if lunar_phase == 'Full':
   planting_time = True
   sendNotificationToFarmers("It is a full Moon, planting should begin")
 else:
   waitForFullMoon()
+```
+
+Here is another example:
 
+```python 
+from astronomica import *
+PyndyalaCoder = Observer(47.6, -122.2, 'earth')
+print(PyndyalaCoder.mean_anomaly())
 ```
 
 ## Methods
 
 ```python
 fahrenheit_to_celsius(f)
 celsius_to_fahrenheit(c)
```

### Comparing `astronomica-0.0.6/README.md` & `astronomica-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 # astronomica
 
 ## Introduction and Purpose
+
 <b>Astronomica</b> is a simple python library based on formulas pioneered at https://www.aa.quae.nl/en/reken/zonpositie.html, and https://astronomica.w3spaces.com/. Scroll below to check out the documentation. This library does not depend on Astropy or Skyfield, but requires their installation for conversion purposes - some of our functions include interoperability of libraries - skyfield units to astropy units, etc.
 
 ### Note of Usage:
 <b>Astronomica is 100% free</b>!! It is also <b>driven by the <i>community</i></b>, so we welcome tips, bug fixes, and more methods added by users and the general python & astronomy community. You can also join our reddit community at https://www.reddit.com/r/pythonlibraries/ 
 
 
 ## Usage:
 Here is a very simple usage example of Astronomica:
 
 ```python
-
 from astronomica import *
-
 lunar_phase = getLunarPhase()
 planting_time = False
 if lunar_phase == 'Full':
   planting_time = True
   sendNotificationToFarmers("It is a full Moon, planting should begin")
 else:
   waitForFullMoon()
+```
+
+Here is another example:
 
+```python 
+from astronomica import *
+PyndyalaCoder = Observer(47.6, -122.2, 'earth')
+print(PyndyalaCoder.mean_anomaly())
 ```
 
 ## Methods
 
 ```python
 fahrenheit_to_celsius(f)
 celsius_to_fahrenheit(c)
```

### Comparing `astronomica-0.0.6/astronomica/astronomica.py` & `astronomica-0.0.7/astronomica/astronomica.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,177 +1,43 @@
-# import required libraries (math and datetime are always required, because of their uses)
-import math
+import os
 import datetime
+import math
 from astroquery.simbad import Simbad
 import requests
-import os
-
 
+"""
+***********************
+***********************
+** TIME CALCULATIONS **
+***********************
+***********************
+"""
+# returns the time as an str: like 5:55:0 where 5 is hour, 55 is minute, 0 is second
 def time():
     time_str = os.popen('date +%H:%M:%S').read().strip()
     return time_str
 
-
+# returns the date as an str: like 4/7/23 where 4 is the month, 7 is the day, 23 is the year
 def date():
     date_str = os.popen('date +%D').read().strip()
     return date_str
 
-
-def decimal_hours():
-    time_str = time()
-    new_time = time_str.split(':')
-    dec_hours = int(new_time[0]) + (int(new_time[1]) / 60) + (int(new_time[2]) / 3600)
-    return dec_hours
-
-
-class DateObject:
-    def __init__(self, data):
-        self.__dict__ = data
-        
-class Date:
-    def __init__(self):
-        self.minute = None
-        self.second = None
-        self.hour = None
-        self.day = None
-        self.year = None
-        self.month = None
-
-    def now(self):
-        hr, min, second = [int(part) for part in time().split(':')]
-        month, day, year = [int(part) for part in date().split('/')]
-        self.month, self.year, self.day = month, year, day
-        self.minute, self.second, self.hour = min, second, hr
-        current_time = {
-            'hour': self.hour,
-            'minute': self.minute,
-            'second': self.second,
-            'day': self.day,
-            'month': self.month,
-            'year': self.year,
-        }
-        return DateObject(current_time)
-    
-class LST:
-    def __init__(self, data):
-        self.__dict__ = data
-
-
-def definition_of(word):
-    # make a request to the Wikipedia API
-    response = requests.get(f"https://en.wikipedia.org/api/rest_v1/page/summary/{word}")
-    # check if the request was successful
-    if response.status_code != 200:
-        return "Sorry, I could not find information on that word."
-    # extract the summary text from the response
-    summary = response.json()['extract']
-    return summary
-
-
-def get_object_equatorial_coords(obj_name):
-    """
-    :param obj_name: name of the SIMBAD object
-    :return: the RA and declination of the object
-    """
-    # Query the SIMBAD database for the object
-    result_table = Simbad.query_object(obj_name)
-    # Extract the RA and Dec coordinates from the result table
-    ra = result_table['RA'][0]
-    dec = result_table['DEC'][0]
-    # Return the RA and Dec coordinates as floats
-    return ra, dec
-
-
-def get_spectral_info(obj_name):
-    """
-    Query the SIMBAD database for spectral information on the given object.
-
-    :param obj_name: Name or identifier of the object.
-    :return: A dictionary with the spectral information for the object.
-    """
-    # Query the SIMBAD database for the object
-    result_table = Simbad.query_object(obj_name)
-    # Check if the result table is empty
-    if result_table is None:
-        return {'error': f'No results found for object {obj_name}'}
-    # Check if the spectral type is present in the result table
-    if 'SP_TYPE' in result_table.columns:
-        spectral_type = result_table['SP_TYPE'][0]
-    else:
-        spectral_type = 'N/A'
-    # Check if the spectral class is present in the result table
-    if 'SP_BIBCODE' in result_table.columns:
-        spectral_class = result_table['SP_BIBCODE'][0]
-    else:
-        spectral_class = 'N/A'
-    # Return the spectral information as a dictionary
-    return {'spectral_type': spectral_type, 'spectral_class': spectral_class}
-
-
+# given a time, return the local julian date (i.e, 2451545 (Jan 1st 2000))
 def local_julian_date(date=datetime.datetime.now()):
     time = date.timestamp() * 1000  # Convert to milliseconds
     tzoffset = date.utcoffset().total_seconds() // 60 if date.utcoffset() is not None else 0  # Convert to minutes
     return (time / 86400000) - (tzoffset / 1440) + 2440587.5  # return the Julian Date
 
-
-J1970 = 2440588
-dayMs = 24 * 60 * 60 * 1000
-
-
+# given a julian date, it converts it to a datetime time
 def fromJulian(j):
+    J1970 = 2440588
+    dayMs = 24 * 60 * 60 * 1000
     return datetime.datetime.fromtimestamp((j + 0.5 - J1970) * dayMs / 1000)
 
-
-LUNAR_MONTH = 29.530588853
-
-
-def get_lunar_age():
-    percent = get_lunar_age_percent()
-    age = percent * LUNAR_MONTH
-    return age
-
-
-def get_lunar_age_percent():
-    julian_date = local_julian_date()
-    return normalize((julian_date - 2451550.1) / LUNAR_MONTH)
-
-
-def normalize(value):
-    value = value - int(value)
-    if value < 0:
-        value = value + 1
-    return value
-
-
-def getLunarPhase(date=datetime.datetime.now()):
-    age = get_lunar_age()
-    if age < 1.84566:
-        return "New"
-    elif age < 5.53699:
-        return "Waxing Crescent"
-    elif age < 9.22831:
-        return "First Quarter"
-    elif age < 12.91963:
-        return "Waxing Gibbous"
-    elif age < 16.61096:
-        return "Full"
-    elif age < 20.30228:
-        return "Waning Gibbous"
-    elif age < 23.99361:
-        return "Last Quarter"
-    elif age < 27.68493:
-        return "Waning Crescent"
-    return "New"
-
-
-def solarMeanAnomaly(d):
-    rad = math.pi / 180.0
-    return rad * (357.5291 + 0.98560028 * d)
-
-
+# returns the amount of days since the J2000 epoch
 def daysSinceJ2000():
     # get current date and time in UTC
     now = datetime.datetime.utcnow()
     year = now.year
     month = now.month
     day = now.day
     hour = now.hour
@@ -187,34 +53,28 @@
     JD = 367 * Y - math.floor(7 * (Y + math.floor((M + 9) / 12)) / 4) + math.floor(
         275 * M / 9) + D + 1721013.5 + UT / 24
 
     # calculate number of days since J2000.0
     days = (JD - 2451545.0) + (UT - 12) / 24
     return days
 
-
-def declination(l, b):
-    e = math.radians(23.4397)  # obliquity of the ecliptic in degrees
-    return math.asin(
-        math.sin(math.radians(b)) * math.cos(e) + math.cos(math.radians(b)) * math.sin(e) * math.sin(math.radians(l)))
-
-
+# helper method for the local sidereal time calculation
 def sign(x):
     if x > 0:
         return 1
     elif x < 0:
         return -1
     else:
         return 0
 
-
+# get the decimal hours based on a datetime.datetime.now() object
 def decimalhours(now):
     return (((now.second / 60) + now.minute) / 60) + now.hour
 
-
+# helper method for the local sidereal time
 def gst(jd, dechours):
     S = jd - 2451545
     T = S / 36525
     T0 = 6.697374558 + (2400.051336 * T) + (0.000025862 * T ** 2)
     if T0 < 0:
         T0 = (T0 + abs(T0) // 24 * 24) % 24
     else:
@@ -222,16 +82,16 @@
     T0 = T0 + (dechours * 1.002737909)
     if T0 < 0:
         T0 = T0 + 24
     if T0 > 24:
         T0 = T0 - 24
     return T0
 
-
-def localSiderealTime(long):
+# returns the local sidereal time
+def local_sidereal_time(long):
     now = datetime.datetime.utcnow()
     jd = local_julian_date()
     dechours = decimalhours(now)
     gstime = gst(jd, dechours)
     LONGITUDE = long
     utcdiff = math.fabs(LONGITUDE) / 15
     if sign(LONGITUDE) == -1:
@@ -250,356 +110,363 @@
 
     times = {
         "raw": raw,
         "hour": h,
         "minute": m,
         "second": s
     }
-    return LST(times)
+    return times
+
 
+"""
+****************
+****************
+GENERAL SUN CALC
+****************
+****************
+"""
 
-def eclipticLongitude(M):
+def declination(l, b):
+    e = math.radians(23.4397)  # obliquity of the ecliptic in degrees
+    return math.asin(
+        math.sin(math.radians(b)) * math.cos(e) + math.cos(math.radians(b)) * math.sin(e) * math.sin(math.radians(l)))
+
+def solar_mean_anomaly(d):
+    """
+    :param d: days since J2000
+    :return: the solar mean anomaly for EARTH (other planets in other function)
+    """
     rad = math.pi / 180.0
-    PI = math.pi
+    return rad * (357.5291 + 0.98560028 * d)
 
+def ecliptic_longitude(M):
+    """
+    :param M: solar mean anomaly
+    :return: the ecliptic longitude of the sun
+    """
+    rad = math.pi / 180.0
+    PI = math.pi
     C = rad * (1.9148 * math.sin(M) + 0.02 * math.sin(2 * M) + 0.0003 * math.sin(3 * M))  # equation of center
     P = rad * 102.9372  # perihelion of the Earth
-
     return M + C + P + PI
 
-
-def solarHourAngle(longitude, lst):
+def solar_hour_angle(longitude, lst):
     """Calculate the solar hour angle for a given longitude and local sidereal time."""
     # Convert longitude and LST to radians
     longitude = math.radians(longitude)
     lst = math.radians(lst)
     # Calculate the solar noon for the given longitude
     solarNoon = longitude + (12 - 12 * 4.0 / 1440) * math.radians(360) / 24
     # Calculate the solar hour angle
     hourAngle = lst - solarNoon
     return hourAngle
 
-
 def altitude(lat, long):
+    """
+    :param lat: the latitude of the user
+    :param long: the longitude of the user
+    :return: the altitude of the sun
+    """
     long = -long
     d = daysSinceJ2000()
-    M = solarMeanAnomaly(d)
-    L = eclipticLongitude(M)
+    M = solar_mean_anomaly(d)
+    L = ecliptic_longitude(M)
     dec = declination(L, 0)
-    H = solarHourAngle(long, localSiderealTime(long).raw)
+    H = solar_hour_angle(long, local_sidereal_time(long)['raw'])
     a = math.asin(math.sin(lat) * math.sin(dec) + math.cos(lat) * math.cos(dec) * math.cos(H))
     return math.degrees(a)
 
-
 def azimuth(lat, long):
+    """
+    :param lat: latitude of the user
+    :param long: longitude of the user
+    :return: the azimuth of the sun in degrees
+    """
     long = -long
     d = daysSinceJ2000()
-    M = solarMeanAnomaly(d)
-    L = eclipticLongitude(M)
-    H = solarHourAngle(long, localSiderealTime(long).raw)
+    M = solar_mean_anomaly(d)
+    L = ecliptic_longitude(M)
+    H = solar_hour_angle(long, local_sidereal_time(long)['raw'])
     dec = declination(L, 0)
     return math.degrees(math.atan2(math.sin(H), math.cos(H) * math.sin(lat) - math.tan(dec) * math.cos(lat)))
 
+# returns the mean anomaly of a planet
+def mean_anomaly(planet):
+    # formula from https://www.aa.quae.nl/en/reken/zonpositie.html
+    # formula is M = (M0 + M1 * (J - J2000)) mod 360˚
+    J2000 = 2451545
+    m_list = [
+        (174.7948, 4.09233445),
+        (50.4161, 1.60213034),
+        (357.5291, 0.98560028),
+        (19.3730, 0.52402068),
+        (20.0202, 0.08308529),
+        (317.0207, 0.03344414),
+        (141.0498, 0.01172834),
+        (256.2250, 0.00598103),
+        (14.882, 0.00396),
+    ]
+    planetMap = {
+        'mercury': 0,
+        'venus': 1,
+        'earth': 2,
+        'mars': 3,
+        'jupiter': 4,
+        'saturn': 5,
+        'uranus': 6,
+        'neptune': 7,
+        'pluto': 8,
+    }
+    plan_number = planetMap.get(planet, 2)  # if the planet is not found, calculate for earth
+    m_row = m_list[plan_number]
+    M = (m_row[0] + m_row[1] * (local_julian_date() - J2000)) % 360
+    return M
+
+# the equation of center for any planet
+def equation_of_center(planet):
+    c_dict = {
+        "mercury": [23.4400, 2.9818, 0.5255, 0.1058, 0.0241, 0.0055],  # 0.0026 is the maximum error
+        "venus": [0.7758, 0.0033, 0, 0, 0, 0],  # 0.0000 is the maximum error
+        "earth": [1.9148, 0.0200, 0.0003, 0, 0, 0],  # 0.0000 is the maximum error
+        "mars": [10.6912, 0.6228, 0.0503, 0.0046, 0.0005, 0],  # 0.0001 is the maximum error
+        "jupiter": [5.5549, 0.1683, 0.0071, 0.0003, 0, 0],  # 0.0001 is the maximum error
+        "saturn": [6.3585, 0.2204, 0.0106, 0.0006, 0, 0],  # 0.0001 is the maximum error
+        "uranus": [5.3042, 0.1534, 0.0062, 0.0003, 0, 0],  # 0.0001 is the maximum error
+        "neptune": [1.0302, 0.0058, 0, 0, 0, 0],  # 0.0001 is the maximum error
+        "pluto": [28.3150, 4.3408, 0.9214, 0.2235, 0.0627, 0.0174]  # 0.0096 is the maximum error
+    }
+    # the formula used is from https://www.aa.quae.nl/en/reken/zonpositie.html#10
+    # c = c1 * sin(m) + c2 * sin(2m) + c3 * sin(3m) + c4 * sin(4m) + c5 * sin(5m) + c6 * sin(6m)
+    c = c_dict.get(planet, [1.9148, 0.0200, 0.0003, 0, 0, 0])
+    m = mean_anomaly(planet)
+    center_eq = c[0] * math.sin(m) + c[1] * math.sin(2 * m) + c[2] * math.sin(3 * m) + c[3] * math.sin(4 * m) + \
+                c[4] * math.sin(5 * m) + c[5] * math.sin(6 * m)
+    return center_eq
+
+# return the true anomaly of the planet
+def true_anomaly(planet):
+    c = equation_of_center(planet)
+    m = mean_anomaly(planet)
+    return m + c  # the equation of center is the correction factor
+
+# return the perihelion and obliquity of a planet
+def get_peri_obli(planet):
+    perihelion_longitude_and_obliquity = [
+        (230.3265, 0.0351),
+        (73.7576, 2.6376),
+        (102.9373, 23.4393),
+        (71.0041, 25.1918),
+        (237.1015, 3.1189),
+        (99.4587, 26.7285),
+        (5.4634, 82.2298),
+        (182.2100, 27.8477),
+        (184.5484, 119.6075),
+    ]
+    planetMap = {
+        'mercury': 0,
+        'venus': 1,
+        'earth': 2,
+        'mars': 3,
+        'jupiter': 4,
+        'saturn': 5,
+        'uranus': 6,
+        'neptune': 7,
+        'pluto': 8,
+    }
+    key = planetMap.get(planet, 2)
+    datatuple = perihelion_longitude_and_obliquity[key]
+    perihelion = datatuple[0]
+    obliquity = math.radians(datatuple[1])
+    return perihelion, obliquity
+
+# return the ecliptical longitude of a planet
+def ecliptical_longitude(planet):
+    peri, obli = get_peri_obli(planet)  # setup information
+    L = mean_anomaly(planet) + peri
+    Lsun = L + 180
+    long = (Lsun + equation_of_center(planet)) % 360
+    return math.radians(long)
+
+# the equatorial coordinates of a planet
+def equatorial_coordinates(planet):
+    long = ecliptical_longitude(planet)
+    peri, obli = get_peri_obli(planet)
+    asun = math.atan2(math.sin(long) * math.cos(obli), math.cos(long))
+    decsun = math.asin(math.sin(long) * math.sin(obli))
+    return {
+        'ra': math.degrees(asun),
+        'dec': math.degrees(decsun)
+    }
 
-class Observer:
-    def __init__(self, latitude, longitude, planet):
-        self.lat = latitude
-        self.long = -longitude  # convert to longitude west from just longitude
-        self.planet = planet
-        self.meanA = None
-        self.ceq = None
-        self.v = None
-        self.perihelion = None
-        self.obliquity = None
-        self.dist = None
-        self.eclipticlong = None
-
-    def julian_date(self):
-        JD = local_julian_date(datetime.datetime.now())
-        return JD
-
-    def mean_anomaly(self):
-        # formula from https://www.aa.quae.nl/en/reken/zonpositie.html
-        # formula is M = (M0 + M1 * (J - J2000)) mod 360˚
-        J2000 = 2451545
-        m_list = [
-            (174.7948, 4.09233445),
-            (50.4161, 1.60213034),
-            (357.5291, 0.98560028),
-            (19.3730, 0.52402068),
-            (20.0202, 0.08308529),
-            (317.0207, 0.03344414),
-            (141.0498, 0.01172834),
-            (256.2250, 0.00598103),
-            (14.882, 0.00396),
-        ]
-        planetMap = {
-            'mercury': 0,
-            'venus': 1,
-            'earth': 2,
-            'mars': 3,
-            'jupiter': 4,
-            'saturn': 5,
-            'uranus': 6,
-            'neptune': 7,
-            'pluto': 8,
-        }
-        plan_number = planetMap.get(self.planet, 2)  # if the planet is not found, calculate for earth
-        m_row = m_list[plan_number]
-        M = (m_row[0] + m_row[1] * (local_julian_date() - J2000)) % 360
-        self.meanA = M
-        return M
-
-    def equation_of_center(self):
-        planet = self.planet
-        c_dict = {
-            "mercury": [23.4400, 2.9818, 0.5255, 0.1058, 0.0241, 0.0055],  # 0.0026 is the maximum error
-            "venus": [0.7758, 0.0033, 0, 0, 0, 0],  # 0.0000 is the maximum error
-            "earth": [1.9148, 0.0200, 0.0003, 0, 0, 0],  # 0.0000 is the maximum error
-            "mars": [10.6912, 0.6228, 0.0503, 0.0046, 0.0005, 0],  # 0.0001 is the maximum error
-            "jupiter": [5.5549, 0.1683, 0.0071, 0.0003, 0, 0],  # 0.0001 is the maximum error
-            "saturn": [6.3585, 0.2204, 0.0106, 0.0006, 0, 0],  # 0.0001 is the maximum error
-            "uranus": [5.3042, 0.1534, 0.0062, 0.0003, 0, 0],  # 0.0001 is the maximum error
-            "neptune": [1.0302, 0.0058, 0, 0, 0, 0],  # 0.0001 is the maximum error
-            "pluto": [28.3150, 4.3408, 0.9214, 0.2235, 0.0627, 0.0174]  # 0.0096 is the maximum error
-        }
-        # the formula used is from https://www.aa.quae.nl/en/reken/zonpositie.html#10
-        # c = c1 * sin(m) + c2 * sin(2m) + c3 * sin(3m) + c4 * sin(4m) + c5 * sin(5m) + c6 * sin(6m)
-        c = c_dict.get(planet, [1.9148, 0.0200, 0.0003, 0, 0, 0])
-        m = self.mean_anomaly()
-        center_eq = c[0] * math.sin(m) + c[1] * math.sin(2 * m) + c[2] * math.sin(3 * m) + c[3] * math.sin(4 * m) + \
-            c[4] * math.sin(5 * m) + c[5] * math.sin(6 * m)
-        self.ceq = center_eq
-        return center_eq
-
-    def true_anomaly(self):
-        c = self.equation_of_center()
-        m = self.mean_anomaly()
-        self.v = c + m
-        return m + c
-
-    def set_perihelion_and_obliquity(self):
-        perihelion_longitude_and_obliquity = [
-            (230.3265, 0.0351),
-            (73.7576, 2.6376),
-            (102.9373, 23.4393),
-            (71.0041, 25.1918),
-            (237.1015, 3.1189),
-            (99.4587, 26.7285),
-            (5.4634, 82.2298),
-            (182.2100, 27.8477),
-            (184.5484, 119.6075),
-        ]
-        planetMap = {
-            'mercury': 0,
-            'venus': 1,
-            'earth': 2,
-            'mars': 3,
-            'jupiter': 4,
-            'saturn': 5,
-            'uranus': 6,
-            'neptune': 7,
-            'pluto': 8,
-        }
-        key = planetMap.get(self.planet, 2)
-        datatuple = perihelion_longitude_and_obliquity[key]
-        self.perihelion = datatuple[0]
-        self.obliquity = math.radians(datatuple[1])
-
-    def ecliptical_longitude(self):
-        self.set_perihelion_and_obliquity()  # setup information
-        peri = self.perihelion
-        L = self.mean_anomaly() + peri
-        Lsun = L + 180
-        long = (Lsun + self.equation_of_center()) % 360
-        self.eclipticlong = math.radians(long)
-        return math.radians(long)
-
-    def equatorial_coordinates(self):
-        long = self.ecliptical_longitude()
-        asun = math.atan2(math.sin(long) * math.cos(self.obliquity), math.cos(long))
-        decsun = math.asin(math.sin(long) * math.sin(self.obliquity))
-        return {
-            'ra': math.degrees(asun),
-            'dec': math.degrees(decsun)
-        }
-
-    def local_solar_transit(self):
-        Jtable = [
-            [45.3497, 11.4556, 0, 175.9386],
-            [52.1268, -0.2516, 0.0099, -116.7505],
-            [0.0009, 0.0053, -0.0068, 1.0000000],
-            [0.9047, 0.0305, -0.0082, 1.027491],
-            [0.3345, 0.0064, 0, 0.4135778],
-            [0.0766, 0.0078, -0.0040, 0.4440276],
-            [0.1260, -0.0106, 0.0850, -0.7183165],
-            [0.3841, 0.0019, -0.0066, 0.6712575],
-            [4.5635, -0.5024, 0.3429, 6.387672]
-        ]
-        planetMap = {
-            'mercury': 0,
-            'venus': 1,
-            'earth': 2,
-            'mars': 3,
-            'jupiter': 4,
-            'saturn': 5,
-            'uranus': 6,
-            'neptune': 7,
-            'pluto': 8,
-        }
-        plannumber = planetMap.get(self.planet, 2)
-        Jrow = Jtable[plannumber]
-        j0 = Jrow[0]
-        j1 = Jrow[1]
-        j2 = Jrow[2]
-        j3 = Jrow[3]
-        nx = (local_julian_date() - 2451545 - j0) / j3 - self.long / 360
-        n = math.floor(nx)
-        jx = local_julian_date() + j3 * (n - nx)
-        self.set_perihelion_and_obliquity()  # setup information
-        peri = self.perihelion
-        L = self.mean_anomaly() + peri
-        lsun = L + 180
-        jtransit = jx + j1 * math.sin(math.radians(self.mean_anomaly())) + j2 * math.sin(2 * math.radians(lsun))
-        return jtransit + 1
-
-    def distance_to_sun(self):
-        square_table = [
-            0.37073,
-            0.72330,
-            0.99972,
-            1.51039,
-            5.19037,
-            9.52547,
-            19.17725,
-            30.10796,
-            37.09129
-        ]
-        e_table = [
-            0.20563,
-            0.00677,
-            0.01671,
-            0.09340,
-            0.04849,
-            0.05551,
-            0.04630,
-            0.00899,
-            0.2490,
-        ]
-        planetMap = {
-            'mercury': 0,
-            'venus': 1,
-            'earth': 2,
-            'mars': 3,
-            'jupiter': 4,
-            'saturn': 5,
-            'uranus': 6,
-            'neptune': 7,
-            'pluto': 8,
-        }
-        key = planetMap.get(self.planet, 2)
-        e = e_table[key]
-        square = square_table[key]
-        r = square / 1 + e * math.cos(self.true_anomaly())
-        self.dist = r
-        return r
-
-    def planet_heliocentric_coordinates(self):
-        square_table = [
-            0.37073,
-            0.72330,
-            0.99972,
-            1.51039,
-            5.19037,
-            9.52547,
-            19.17725,
-            30.10796,
-            37.09129
-        ]
-        e_table = [
-            0.20563,
-            0.00677,
-            0.01671,
-            0.09340,
-            0.04849,
-            0.05551,
-            0.04630,
-            0.00899,
-            0.2490,
-        ]
-        planetMap = {
-            'mercury': 0,
-            'venus': 1,
-            'earth': 2,
-            'mars': 3,
-            'jupiter': 4,
-            'saturn': 5,
-            'uranus': 6,
-            'neptune': 7,
-            'pluto': 8,
-        }
-        r = self.distance_to_sun()
-        horse_table = [
-            48.331,
-            76.680,
-            174.873,
-            49.558,
-            100.464,
-            113.666,
-            74.006,
-            131.784,
-            110.307
-        ]
-        i_table = [
-            7.005,
-            3.395,
-            0.000,
-            1.850,
-            1.303,
-            2.489,
-            0.773,
-            1.770,
-            17.140,
-        ]
-        w_table = [
-            29.125,
-            54.884,
-            288.064,
-            286.502,
-            273.867,
-            339.391,
-            98.999,
-            276.340,
-            113.768
-        ]
-        key = planetMap.get(self.planet, 2)
-        i = i_table[key]
-        horse = horse_table[key]
-        w = w_table[key]
-        v = self.true_anomaly()
-        r = self.distance_to_sun()
-        xplanet = r * (math.cos(horse) * math.cos(w + v) - math.sin(horse) * math.cos(i) * math.sin(w + v))
-        yplanet = r * (math.sin(horse) * math.cos(w + v) + math.cos(horse) * math.cos(i) * math.sin(w + v))
-        zplanet = r * math.sin(i) * math.sin(w + v)
-        return xplanet, yplanet, zplanet
-
-    def planet_geocentric_coordinates(self):
-        earth = Observer(self.lat, self.long, 'earth')
-        x, y, z = earth.planet_heliocentric_coordinates()
-        xplanet, yplanet, zplanet = self.planet_heliocentric_coordinates()
-        return xplanet - x, yplanet - y, zplanet - z
-
-    def planet_geocentric_lat_long(self):
-        x, y, z = self.planet_geocentric_coordinates()
-        change = math.sqrt((x ** 2) + (y ** 2) + (z**2))
-        long = math.atan2(y, x)
-        lat = math.asin(z/change)
-        return lat, long
-
-
+# the solar transit julian of a planet
+def local_solar_transit(planet, long):
+    """
+    :param planet: name of the desired planet
+    :param long: longitude EAST (i.e, west of the prime meridian is negative)
+    :return: the solar transit julian
+    """
+    long = -long
+    Jtable = [
+        [45.3497, 11.4556, 0, 175.9386],
+        [52.1268, -0.2516, 0.0099, -116.7505],
+        [0.0009, 0.0053, -0.0068, 1.0000000],
+        [0.9047, 0.0305, -0.0082, 1.027491],
+        [0.3345, 0.0064, 0, 0.4135778],
+        [0.0766, 0.0078, -0.0040, 0.4440276],
+        [0.1260, -0.0106, 0.0850, -0.7183165],
+        [0.3841, 0.0019, -0.0066, 0.6712575],
+        [4.5635, -0.5024, 0.3429, 6.387672]
+    ]
+    planetMap = {
+        'mercury': 0,
+        'venus': 1,
+        'earth': 2,
+        'mars': 3,
+        'jupiter': 4,
+        'saturn': 5,
+        'uranus': 6,
+        'neptune': 7,
+        'pluto': 8,
+    }
+    plannumber = planetMap.get(planet, 2)
+    Jrow = Jtable[plannumber]
+    j0 = Jrow[0]
+    j1 = Jrow[1]
+    j2 = Jrow[2]
+    j3 = Jrow[3]
+    nx = (local_julian_date() - 2451545 - j0) / j3 - long / 360
+    n = math.floor(nx)
+    jx = local_julian_date() + j3 * (n - nx)
+    peri, obli = get_peri_obli(planet)
+    L = mean_anomaly(planet) + peri
+    lsun = L + 180
+    jtransit = jx + j1 * math.sin(math.radians(mean_anomaly(planet))) + j2 * math.sin(2 * math.radians(lsun))
+    return jtransit + 1
+
+# returns the distance to the sun
+def distance_to_sun(planet):
+    square_table = [
+        0.37073,
+        0.72330,
+        0.99972,
+        1.51039,
+        5.19037,
+        9.52547,
+        19.17725,
+        30.10796,
+        37.09129
+    ]
+    e_table = [
+        0.20563,
+        0.00677,
+        0.01671,
+        0.09340,
+        0.04849,
+        0.05551,
+        0.04630,
+        0.00899,
+        0.2490,
+    ]
+    planetMap = {
+        'mercury': 0,
+        'venus': 1,
+        'earth': 2,
+        'mars': 3,
+        'jupiter': 4,
+        'saturn': 5,
+        'uranus': 6,
+        'neptune': 7,
+        'pluto': 8,
+    }
+    key = planetMap.get(planet, 2)
+    e = e_table[key]
+    square = square_table[key]
+    r = square / 1 + e * math.cos(true_anomaly(planet))
+    return r
+
+# returns the heliocentric coordinates of the planet
+def planet_heliocentric_coordinates(planet):
+    planetMap = {
+        'mercury': 0,
+        'venus': 1,
+        'earth': 2,
+        'mars': 3,
+        'jupiter': 4,
+        'saturn': 5,
+        'uranus': 6,
+        'neptune': 7,
+        'pluto': 8,
+    }
+    r = distance_to_sun(planet)
+    horse_table = [
+        48.331,
+        76.680,
+        174.873,
+        49.558,
+        100.464,
+        113.666,
+        74.006,
+        131.784,
+        110.307
+    ]
+    i_table = [
+        7.005,
+        3.395,
+        0.000,
+        1.850,
+        1.303,
+        2.489,
+        0.773,
+        1.770,
+        17.140,
+    ]
+    w_table = [
+        29.125,
+        54.884,
+        288.064,
+        286.502,
+        273.867,
+        339.391,
+        98.999,
+        276.340,
+        113.768
+    ]
+    key = planetMap.get(planet, 2)
+    i = i_table[key]
+    horse = horse_table[key]
+    w = w_table[key]
+    v = true_anomaly(planet)
+    r = distance_to_sun(planet)
+    xplanet = r * (math.cos(horse) * math.cos(w + v) - math.sin(horse) * math.cos(i) * math.sin(w + v))
+    yplanet = r * (math.sin(horse) * math.cos(w + v) + math.cos(horse) * math.cos(i) * math.sin(w + v))
+    zplanet = r * math.sin(i) * math.sin(w + v)
+    return xplanet, yplanet, zplanet
+
+# returns the geocentric coordinates of the planet
+def planet_geocentric_coordinates(planet):
+    x, y, z = planet_heliocentric_coordinates('earth')
+    xplanet, yplanet, zplanet = planet_heliocentric_coordinates(planet)
+    return xplanet - x, yplanet - y, zplanet - z
+
+# returns the geocentric latitude and longitude of the planet
+def planet_geocentric_lat_long(planet):
+    x, y, z = planet_geocentric_coordinates(planet)
+    change = math.sqrt((x ** 2) + (y ** 2) + (z ** 2))
+    long = math.atan2(y, x)
+    lat = math.asin(z / change)
+    return lat, long
+
+
+"""
+********************
+********************
+**STAR CALCULATION**
+********************
+********************
+"""
 star_catalog = {
     'Sun': 'G2V',
     'Sirius': 'A1V',
     'Betelgeuse': 'M2Iab',
     'Rigel': 'B8Ia',
     'Vega': 'A0Va',
     'Alpha Centauri A': 'G2V',
@@ -660,8 +527,102 @@
 }
 
 
 def map_star(star):
     type = star_catalog.get(star, "Star not currently supported")
     return type
 
+def get_object_equatorial_coords(obj_name):
+    """
+    :param obj_name: name of the SIMBAD object
+    :return: the RA and declination of the object
+    """
+    # Query the SIMBAD database for the object
+    result_table = Simbad.query_object(obj_name)
+    # Extract the RA and Dec coordinates from the result table
+    ra = result_table['RA'][0]
+    dec = result_table['DEC'][0]
+    # Return the RA and Dec coordinates as floats
+    return ra, dec
+
+def definition_of(word):
+    # make a request to the Wikipedia API
+    response = requests.get(f"https://en.wikipedia.org/api/rest_v1/page/summary/{word}")
+    # check if the request was successful
+    if response.status_code != 200:
+        return "Sorry, I could not find information on that word."
+    # extract the summary text from the response
+    summary = response.json()['extract']
+    return summary
+
+"""
+******************
+******************
+*MOON CALCULATION*
+******************
+******************
+"""
+
+LUNAR_MONTH = 29.530588853
+
+def get_lunar_age():
+    percent = get_lunar_age_percent()
+    age = percent * LUNAR_MONTH
+    return age
+
+
+def get_lunar_age_percent():
+    julian_date = local_julian_date()
+    return normalize((julian_date - 2451550.1) / LUNAR_MONTH)
+
+
+def normalize(value):
+    value = value - int(value)
+    if value < 0:
+        value = value + 1
+    return value
+
+
+def getLunarPhase():
+    age = get_lunar_age()
+    if age < 1.84566:
+        return "New"
+    elif age < 5.53699:
+        return "Waxing Crescent"
+    elif age < 9.22831:
+        return "First Quarter"
+    elif age < 12.91963:
+        return "Waxing Gibbous"
+    elif age < 16.61096:
+        return "Full"
+    elif age < 20.30228:
+        return "Waning Gibbous"
+    elif age < 23.99361:
+        return "Last Quarter"
+    elif age < 27.68493:
+        return "Waning Crescent"
+    return "New"
+
+def sin(x):
+    return math.sin(x)
+
+def arcsin(x):
+    return math.asin(x)
+
+def tan(x):
+    return math.tan(x)
+
+def arctan(x):
+    return math.atan(x)
+
+def arctan2(y, x):
+    return math.atan2(y, x)
+
+def sqrt(x):
+    return math.sqrt(x)
+
+def cos(x):
+    return math.cos(x)
+
+def arccos(x):
+    return math.acos(x)
```

### Comparing `astronomica-0.0.6/astronomica/libconversion.py` & `astronomica-0.0.7/astronomica/libconversion.py`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.6/astronomica/suntiming.py` & `astronomica-0.0.7/astronomica/suntiming.py`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.6/astronomica.egg-info/PKG-INFO` & `astronomica-0.0.7/astronomica.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 Metadata-Version: 2.1
 Name: astronomica
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates
 Home-page: https://github.com/PyndyalaCoder/astronomica
 Author: Siddhu Pendyala
 Author-email: elcientifico.pendyala@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/PyndyalaCoder/astronomica/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # astronomica
 
 ## Introduction and Purpose
+
 <b>Astronomica</b> is a simple python library based on formulas pioneered at https://www.aa.quae.nl/en/reken/zonpositie.html, and https://astronomica.w3spaces.com/. Scroll below to check out the documentation. This library does not depend on Astropy or Skyfield, but requires their installation for conversion purposes - some of our functions include interoperability of libraries - skyfield units to astropy units, etc.
 
 ### Note of Usage:
 <b>Astronomica is 100% free</b>!! It is also <b>driven by the <i>community</i></b>, so we welcome tips, bug fixes, and more methods added by users and the general python & astronomy community. You can also join our reddit community at https://www.reddit.com/r/pythonlibraries/ 
 
 
 ## Usage:
 Here is a very simple usage example of Astronomica:
 
 ```python
-
 from astronomica import *
-
 lunar_phase = getLunarPhase()
 planting_time = False
 if lunar_phase == 'Full':
   planting_time = True
   sendNotificationToFarmers("It is a full Moon, planting should begin")
 else:
   waitForFullMoon()
+```
+
+Here is another example:
 
+```python 
+from astronomica import *
+PyndyalaCoder = Observer(47.6, -122.2, 'earth')
+print(PyndyalaCoder.mean_anomaly())
 ```
 
 ## Methods
 
 ```python
 fahrenheit_to_celsius(f)
 celsius_to_fahrenheit(c)
```

### Comparing `astronomica-0.0.6/setup.py` & `astronomica-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='astronomica',
-    version='0.0.6',
+    version='0.0.7',
     author='Siddhu Pendyala',
     author_email='elcientifico.pendyala@gmail.com',
     description='A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates',
     long_description = long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/PyndyalaCoder/astronomica',
     project_urls = {
```

