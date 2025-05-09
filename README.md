#date and time and calender epoch time
from datetime import datetime
now=datetime.now()
print("current time:",now)
print("Date:",now.date())
print("Time:",now.time())

import calendar
year=2025
print(calendar.calendar(year))

import calendar
year=2024
print("is leap year",calendar.isleap(year))

#finding leapyear 
import calendar
leaps=calendar.leapdays(1925,2025)
print(leaps,end='')

#difference in days
from datetime import date
d1=date(2025,5,9)
d2=date(2024,1,1)
difference=d1-d2
print("difference in dates:",difference.days)

#day abbreviation (upper case)
from datetime import date
today=date.today()
name=today.strftime("%A")
print("Today: ",name)

#day abbreviation (lower case)
from datetime import date
today=date.today()
name=today.strftime("%a")
print("Today: ",name)
