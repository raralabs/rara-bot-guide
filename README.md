# 1. How To Use

We can directly message **Rara bot** in our workspace using following commands.

### 1.1 Commands

* `/out`:- Command to work with recording absent data. Commands available:
    * `/out` - > Give modal to register absent details
    * `/out -d n` where n is *number of day* ->  Record details *n* day from today, reason will be *null*
    * `/out -d n "I am travelling"`-> Record details *n* day from today, reason for *leave*
    * `/out -undo` -> Leave will be removed but with limit (default: 30 minutes)
    
* `/out-today`:- Gets all name of member who are absent today.

* `/out-month`:- Gets all member who are absent by month.
    * `/out-month` - > All members absent in current month
    * `/out-month -m n` where n is *number of month* -> All members absent by specific month
    * `/out-month -m [m, n]` where m and n is *number of month* -> Data between *m* and *n* (including *both*)
    * `/out-month -m n false`-> All members absent by specific month, _false_ represent include weekends or not
    * `/out-month -me` -> Total leaves by current user in current month
    Note:- `-me` takes same values as by `-m`.
    
* `/out-year`:- Gets all member who are absent by year.
    * `/out-year` - > All members absent in current year
    * `/out-year -y n` where n is *number of year* -> All members absent by specific year
    * `/out-year -y [m, n]` where m and n is *number of year* -> Data between *m* and *n* (including *both*)
    * `/out-year -y n false`-> All members absent by specific year, _false_ represent include weekends or not
    * `/out-year -me` -> Total leaves by current user in current year
    Note:- `-me` takes same values as by `-y`.