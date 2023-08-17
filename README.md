# NJIT Academic Calendar Converter
This is an academic calendar converter that can be added to your Google Calendar. I used the academic calendar from the "Academic Calendars" tab of the Office of the Registrar's page on NJIT's website, the link can be found here: https://www.njit.edu/registrar/calendars. To look at other academic calendars besides the one for the upcoming semester, you can use the link provided and scroll down to the bottom.

## :scroll: Table of Contents
- [Introduction](https://github.com/gorbe2002/njit-academic-calendar-converter#njit-academic-calendar-converter)
- [:question: How can you use this?](https://github.com/gorbe2002/njit-academic-calendar-converter/edit/main/README.md#question-how-can-you-use-this)
- [:notebook: My Process](https://github.com/gorbe2002/njit-academic-calendar-converter/edit/main/README.md#my-process)
- [:thought_balloon: Final Notes](https://github.com/gorbe2002/njit-academic-calendar-converter/edit/main/README.md#thought_balloon-final-notes)

## :question: How can you use this?
- One way to use this would be to download the .csv file from the documents above corresponding to which calendar you want, open your Google Calendar, click on the plus sign next to "Other calendars" on the left side, click "Import", select the downloaded .csv file to add to your calendar, and then click on "Import."
- Another way to use this would be to convert the .csv file into a .iCal file using this converter: https://csv-to-ical.chimbori.com/preview-ics. You would follow almost all the steps as above, except you would select the downloaded .iCal file to add to your calendar. (I wouldn't recommend this way, however, because one of the rows in the "Subject" column, ("Last Day for 90% Refund..."), gets split up when importing the table, so you would lose this event in your calendar.)

## :notebook: My Process
Firstly, I did everything on Google Sheets, so a lot of functions were used. Also, the format to be able to import the event in Google Calendar or even to convert it to .iCal has to be very specific (specifically: in mm/dd/yyyy format), which is why I had to make a reference table (MonthsAsNumbers) to convert the months to numbers and had Zero-Padded Columns for the months and days. After converting the necessary data, I was then able to convert the Google Sheets files into a .csv file, where I was able to import it in my calendar on Google Calendar.

## :thought_balloon: Final Notes
- The "Subject" and "Start Date" columns are mandatory to have to be able to add an event to your calendar.
- The "All Day" column being set to True is just a visually appealing add-on, so it's not mandatory to include.

Last Updated: August 2023
