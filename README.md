#### Scheduling App for Wechat Users

* PostgreSQL
* API-only RoR app
* Heroku backend server
* Wechat Oauth
* Google Cloud Service(storage, geo-location)
* Vue-js front-end
* 3rd party payment processing(OTT Pay)

<img src="./pic/designer_homepage.png" height="400px" />

## index page of created by designer

* customer could choose one of the 8 sports
* workout is the only working feature
* the other 7 sports would trigger a ballot event to collects user data to help the client to determine which sport to be added next

<p float="left">
  <img src="./pic/customer_schedule_entry.jpg" margin="20px" width="225px" />
  <img src="./pic/customer_date_entry.jpg" margin="20px" width="225px" />
  <img src="./pic/customer_time_entry.jpg" margin="20px" width="225px" />
</p>

* Customer choose date(with or without calender), start time(end time auto generated), address(use current location/enter manually)
* Address then geo-located using Google Cloud Service
* database would then filter out all the available coach within 5km from user location

<img src="./pic/customer_appointment_list.png" float="left" margin="20px" height="400px" />

* customer view of the appointments list

<kbd>
  <img src="./pic/admin_employee_interface.png" float="left" margin="20px" height="400px" />
</kbd>

* admin can manage current employee, suspend/activate employee working status
* admin can create employee notes for internal use(with auto-generate timestamp)
* change employee profile pic(override the original one that's captured from wechat)
* inspect the employee's certificate/resume which was saved in Google Cloud Storage

<kbd>
  <img src="./pic/applicant_management.png" float="left" margin="20px" height="400px" />
</kbd>

* admin can accept/reject applicant's application
* admin can view the certificate/resume uploaded by the applicant
* admin can add note to each applicant(with auto-generate timestamp)