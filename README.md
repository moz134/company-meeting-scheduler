

# company-meeting-scheduler


Company Meeting Scheduler

Fetch the data from the following endpoint http://fathomless-shelf-5846.herokuapp.com/api/schedule?date="25/09/2021" 
by querying for a particular date in dd/mm/yyyy format.
You will receive an unordered dictionary of already scheduled meetings(booked slots) for that date.

Create a single page application that will list the scheduled meetings ordered by start time for a give date. When no date is selected or on first launch, fetch the schedule for today’s date.

Portrait Mode: HOME@2x.png
Landscape Mode:  HOME Landscape@2x.png


Settings: User should be able to configure following options in app locally.
Working Days - choose from Mon-Sun
Company Timings (eg. 9am-5pm i.e working hours) - this will be used for showing the possible time range that user can choose from while scheduling the meeting.
Slot interval(in minutes): possible values would be 30 and 60. So if interval is chosen to be 30 then start_time options would be 9, 9:30, 10, 10:30 etc.. similarly end_time options would be set.
UI is not mandatory for the same, can provide configuration option in code itself

NEXT Button: Tapping over this button will fetch the scheduled meetings (request from API) for next date

PREV Button: Tapping over this button will fetch the scheduled meeting for prev date (request from API)

Next & Prev buttons should skip non working days, so if weekends are off and it's a friday then clicking next should query for the next working day i.e monday.

Store the results locally only for the last fetched date from API (and not all the dates that user looks for). When app is reopened or user navigates back to this screen show the stored results (without making an API request)

