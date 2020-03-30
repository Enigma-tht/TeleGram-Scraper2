# TeleGram-Scraper2
инструмент для удаления группы телеграмм получить всю информацию о членах  API Setup
Go to http://my.telegram.org and log in.
Click on API development tools and fill the required fields.
put app name you want & select other in platform Example :
copy "api_id" & "api_hash" after clicking create app ( will be used in setup.py )
• How To Install and Use
$ pkg install -y git python

$ git clone https://github.com/genprokyror/TeleGram-Scraper2

$ cd TeleGram-Scraper2

Install requierments
$ python3 setup.py -i

setup configration file ( apiID, apiHASH )
$ python3 setup.py -c

To Genrate User Data
$ python3 scraper.py

( members.csv is default if you changed name use it )
Send Bulk sms To Collected Data
$ python3 smsbot.py members.csv

add users to your group ( as per api limitation 50 users a day )
$ python3 add2group.py members.csv
