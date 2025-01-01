# Python Calendar Calculations
Calendrical calculations allowing date conversion between the [Gregorian](https://en.wikipedia.org/wiki/Gregorian_calendar), [Revised Julian \(Milanković\)](https://en.wikipedia.org/wiki/Revised_Julian_calendar), and [Julian](https://en.wikipedia.org/wiki/Julian_calendar) calendars.

These functions use the concept of a Chronological Julian Day Number \(CJDN\). Using these functions, a date on any of the Gregorian, Revised Julian (Milanković), or Julian calendars may be converted to a date on one of the other of those calendars.

The Chronological Julian Day Number is a whole number representing a day.
 Its day begins at 00:00 Local Time. The zero point for a Julian Date \(JD 0.0\) corresponds to 12.00 UTC, 1 January -4712 \(i.e. 4713&nbsp;BC\). The zero point for the CJDN is 1 January -4712 \(the whole day in local time\). For more information see: [Julian Day](http://aa.quae.nl/en/reken/juliaansedag.html) .

This Python script imports `argparse`, `datetime` and two functions \(`floor` and `fmod`\) from the `math` package. The script is written in Python 3 \(minimum version 0x030000F0\). As most of it consists of mathematical calculations, I do not envisage any issues using the functions in an earlier version of Python.

```
usage: MattaCalendarCalculations.py [-h] [-t {G,J,M}] year month day

positional arguments:
  year
  month
  day

options:
  -h, --help            show this help message and exit
  -t {G,J,M}, --type {G,J,M}
                        calendar type for input date: G - Grigorian; J - Julian; M - Revised julian (Milanković)
```
