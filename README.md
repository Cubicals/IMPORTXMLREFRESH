In order to import this code go to Extensions-apps script and paste it in Code.gs 

you will need to change "your spreadsheet id" you can find your id in the url "docs.gogle.com/spreadsheets/d/1DcYzDRL0ow6v5n_LZV5TVLcZywkuuGYs87aUbM6-KYw/edit?gid=1973484212#gid=1973484212"
example my id would be "1DcYzDRL0ow6v5n_LZV5TVLcZywkuuGYs87aUbM6-KYw"                                                

 As this gets sheets by name make sure you put the right sheet in because thats the one it will update. "var sheet = ss.getSheetByName("SHEET YOU WANT TO UPDATE");"

 // Show last updated time on sheet somewhere
  sheet.getRange(7,1).setValue("last updated at " + now.toLocaleTimeString()) make sure this isnt overriding your data "7,1" would put the time stamp in collom 7 row A

  AS YOU CLICK TO RUN THIS IT WILL ASK YOU TO LOG IN AND YOU WILL GET A POP UP SAYING IT HASNT BEEN ALLOWED CLICK ADVANCED AND ALLOW IT TO RUN.

  The code puts script in the menu so you can click it there to run when you want.
       

to set a trigger left side of the menu there will be a clock that says triggers click on that and hit the + add trigger
select function- Should be "Refreshimports"
event sorce- time-driven
time based trigger- hour
select interval
NOTE: depending on how many imports you have you dont want this to trigger every min as google will slow it down.






























'
