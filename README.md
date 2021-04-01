Quick Quiz – Laravel Quiz and Exam System
Documentation by “Media City” v2.2
Portfolio Media City
version: 2.2
created: 20/12/2017
updated: 05/09/2019
by: Media City
mediacity.co.in
email: sudhirchechani@gmail.com
Thank you for purchasing this script. For further questions please contact us through ThemeForest or leave an comment. We'd love respond to you!

Overview
Don’t you think you should upgrade the test / exam pattern of your institute?

As we all know we moving our steps very fast with the new-new technology day by day. So why? to adopt the old pattern of taking exams. Better to update your test & exam segment forms with our developed platform named “Quick Quiz”.

Read Digital + Test Digital = You will save your time as well as your capital.

“Quick Quiz” is a platform for Schools, Colleges, Institute & Coaching Centers. With the help of this platform, you can take Online-Offline Exams, Quiz, Test, Quiz Competition, Challenges etc.

Key Features
Quiz and Exam System
Support Lan
Admin Panel
Login System
Secure login and change password
Secure password
Faq Pages
Custom Pages
Mail Setting through Admin Panel
PayPal Payment Gateway
Paid And Free Quiz
Bootstrap 3 Framework
Vue Js
Based on 1170px grid
W3C Valid Markup
Smooth Transition Effects
Free Icon Fonts
Font Awesome Icons
Google Fonts
Cross Browser Compatible
Mobile and Tablet Support
Responsive Design
Documentation Include
Unique and Exclusive Idea
Unique and Creative Project
Installation
Introduction
Before install make sure you have the proper server requirements

PHP 7.2 or greater
OpenSSL PHP Extension 
PHP Fileinfo extension
PHP Zip Archive
	
File and folder permissions

/bootstrap        775
/public/	  775
/storage          775
	
Installation with Apache
Before installing, make sure mod_rewrite is enabled.

Unzip the source file

cd /home/user/
unzip quickquiz.zip
	
/home/user/quickquiz, you can configure Apache virtual host as follows (remember to point the DocumentRoot to the public folder of the source)

<VirtualHost *:80>
	ServerName yoursite.com
	DocumentRoot "/home/user/quickquiz/public"
	Options Indexes FollowSymLinks
	<Directory "/home/user/quickquiz/public">
		AllowOverride All
		Require all granted
	</Directory>
</VirtualHost>
	
Change the director/file’s owner to Apache’s running user (www-data for example), to make sure it has proper permission on your source files

sudo chown www-data:www-data -R /home/user/quickquiz
sudo chmod 775 -R /home/user/quickquiz
	
Then restart Apache.

Shared Hosting Install
Consider that this is the webroot folder for your quickquiz website: /home/myusername/public_html/

Put all the main folder’s files in your quickquiz website at /home/myusername/public_html/

Create MySQL database, add user to it with full permissions. Import (Database -> quiz_db.sql ) quiz_db.sql file in created Database.

open .env file and Fill database Details.

DB_DATABASE=
DB_USERNAME=
DB_PASSWORD=
You are done.

For Cpanel Installation Demo Video Mail Your Purchase Code.
Mail Settings
For Email Sending When User Register and forgot password.

Open and edit .env file.

MAIL_DRIVER=smtp  (Some time sendmail)
MAIL_HOST=smtp.gmail.com (For Gmail = smtp.gmail.com)
MAIL_PORT=2525  (For Gmail = 465)
MAIL_USERNAME=youremailid
MAIL_PASSWORD=yourpassword
MAIL_ENCRYPTION=null  (For Gmail = ssl)
Mail Chimp Or Subscribe Newsletter Settings
For mail chimp or subscribe newsletter.

Open and edit .env file.

MAILCHIMP_API_KEY=yourapikey
MAILCHIMP_LIST_ID=yourlistid
Open and edit  app -> Http -> Controllers -> mailChimpController.php

protected $listId = 'yourmailchimplistid';
Remove Public From URL
To remove public from URL create .htaccess file in root folder and write following code.

<IfModule mod_rewrite.c>
	RewriteEngine On 
	RewriteRule ^(.*)$ public/$1 [L]
</IfModule>
For more detail read article : https://stackoverflow.com/questions/23837933/how-can-i-remove-public-index-php-in-the-url-generated-laravel

Debug Mode
Debug mode will help you to track the error on your website. It is not all preferred to turn the debug mode on live site for very long time.

How to turn debug mode on

Login to you FTP account.
Open and edit .env file.
Change

APP_DEBUG=false
To

APP_DEBUG=true
Save and upload the file.
false means debug mode is OFF
true means debug mode is ON

General Settings
User Register and Reset Password Show Error
Reset password error show due to you forget add mail details in .env file.
Mail Settings
For Email Sending.

Open and edit .env file.

MAIL_DRIVER=smtp
MAIL_HOST=smtp.gmail.com (For Gmail = smtp.gmail.com)
MAIL_PORT=2525 (For Gmail = 465)
MAIL_USERNAME=youremailid
MAIL_PASSWORD=yourpassword
MAIL_ENCRYPTION=null (For Gmail = ssl)

Best Image Size
Logo : 1440 X 675
HTTP 500 Error
This error show to PHP version.
Please make sure you select PHP version 7.1.
Please make sure your database all details is correct.
HTTP 500 Error

Default Login Details
Admin:

Username: admin@info.com
Password: 123456

PayPal Settings
For Paypal payment gateway You Need Paypal Key. For Key Go To: https://paypal.com/

Go to .env file and fill following details
PAYPAL_CLIENT_ID=yourclientid
PAYPAL_SECRET_ID=yoursecretid
PAYPAL_MODE=paypalmode (sandbox or live)
Note : All your test complete then make Paypal to live mode, Paypal Sandbox Mode user and plan not support to live mode.
Please make new user and plan after Paypal live.
Paypal not support $0 plan it's need at least $1.
If Showing Error Check Currency Code In Site Settings -> General Settings.
Updates
05/09/2019 ( Version 2.2 )
- Results Issue Fixed
- Each Student Reset Answer
- Answer Explanation Issue Fixed
20/08/2019 ( Version 2.1 )
- Login & Register UI Issue
- Fix Footer Bar Issue
- Fix Question Not Adding Bug
- Show Answers Repeat Issue Fixed
- Change Password Issue Bug Fixed
- Add New User Through Admin Bug Fixed
28/05/2019 ( Version 2.0 )
- Social Icons Add
- Forgot Password Add
- Custom Pages
- Faq's
- Copyright Text Change
- Mail Setting Through Admin
- Payment History
- PayPal Payment Gateway Add
- Free And Paid Quiz Option
- Right Click & Inspect Element Disable
- Enable / Disable Show Answers
- Improve Change Password
- Delete Answer Each Quiz
- Git Lab Login (Twitter, Git Hub, Bit Bucket & Google)
- Social Login (Facebook & Google)
18 January 2019
- Hours Time Issue Resolved
- Question Again Given Issue Resolved
- Validate W3C
- Fixing Minor Bugs
10 June 2018
- Student Reports Show Issue resolved.
- Student Marks Issue Resolve
- Arrange Menu Proper Way
- Provide Proper descriptions and Instructions
- Footer Copyright, Title Issue Resolved
- Fixing Minor Bugs
05 January 2018
- Bulk Question Importer
- Student Marks Issue Resolve
22 December 2017
- Images Option In Questions
- YouTube & Vemo Video Option In Questions
- Students See Result After Quiz
Update Process
Note: Before Update Take Backup of All Files And Database. Make .zip file and download all file, Go To phpmyadmin and select your database and export it.
Copy All files and paste to you folder replace file. Only be careful when replace files in public folder and .env file. Any user customize design and code please do not update. For database do not import all tables. Please Do not import whole database file, only new user required to update whole database.

Update Version 2.0
Copy All files of folder and paste to you folder replace file, only be careful when replace files in public folder. Database old is work fine but need some columns and tables.

1.	Add show_ans, amount column in topics table. Make both Integer and NULL.
2.	Add right_setting, element_setting, fb_login, gitlab_login, google_login column in settings table. Make all boolean and NULL.
3.	Add google_id, facebook_id column in users table. Make both column unique and NULL.
4.	Remove tests table. It's not required.
5.	Create New Table topic_user, faq, copyrighttexts, configs, social_icons and pages.
Note: You Can Import Table From Database -> Old Users Update -> quickquiz_2_0.sql.

Note: You Can not Import Columns, You need to create it Manually.
Update Version 2.1
First Update 2.0 then update it. Copy All files of folder and paste to you folder replace file, only be careful when replace files in public folder and .env file. Any user customize design and code please do not update.

Note: Before Update Take Backup of All Files And Database. Make .zip file and download all file, Go To phpmyadmin and select your database and export it.


Update Version 2.2
First Update 2.0 then update it. Copy All files of folder and paste to you folder replace file, only be careful when replace files in public folder and .env file. Any user customize design and code please do not update.

Note: Before Update Take Backup of All Files And Database. Make .zip file and download all file, Go To phpmyadmin and select your database and export it.
