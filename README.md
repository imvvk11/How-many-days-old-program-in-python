# How-many-days-old-program-in-python
output number of days old you are currently from the  time of your dob


"""Here is the code"""


import time #imports time library
from datetime import date

def daysBetweenDates(year1, month1, day1, year2, month2, day2):
    
    today = date(year2, month2, day2)
    
    bDay = date(year1, month1, day1)
    
    time_to_today = abs(bDay - today)
    
    return time_to_today.days

print(daysBetweenDates(1992, 11, 20, 2017, 7, 7))
