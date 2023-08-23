<h4>Check list</h4>

1. “Invite” page<br>
- sending a valid invite code<br>
- sending an invalid invite code<br>
- sending empty field<br>
- sending a valid invite code in CamelCase<br>
- invite code with a space<br>
- inappropriate data types<br>
- successfully validation message (and status code)<br>
- validation error message (and status code)<br><br>

2. “Registration” page<br>
- sending the registration form with valid values<br>
- sending the registration form with one empty required field<br>
- using one unique invite code more than 5 times<br>
- using invalid values for each field:<br>
	- empty field<br>
	- inappropriate data types for each field<br>
	- the first letter is lowercase for “Name” fields<br>
	- the first letter is lowercase for the “Surname” fields<br>
	- using a space inside fields’ values<br>
	- amount of digits in phone numbers less than 8 and more than 16<br>
	- email address without @ character<br>
	- email address without dot<br>
	- email address without domain name<br>
	- email address without username<br>
- successfully validation message (and status code)<br>
- validation error message (and status code)<br><br>

3. “Success” page<br>
- links (on the page, in an email) are compared to each other<br>
- check response fields<br>
- successfully validation message (and status code)<br>
- validation error message (and status code)<br><br>

4. “Certificate” page<br>
- getting the unique certificate by its identifier  <br>
- check response fields<br>
- invalid data: <br>
- id is an integer but doesn’t exist<br>
- id is a character<br>
- letter<br>
- empty value<br>
- successfully validation message <br>
- validation error message if certificate not found<br>


<h5><strong>Test case</strong></h5>
- <a href="https://docs.google.com/spreadsheets/d/1NYSdLCJyl7ICzIMEK1sHL3pvW-ngJJg5/edit?usp=drive_link&ouid=102064553302234595178&rtpof=true&sd=true">Sending request with an invalid data for the name key</a><br>
- <a href="https://docs.google.com/spreadsheets/d/1tgD6m_swB5_1FQYxG0KPlwJqbFE853OK/edit?usp=drive_link&ouid=102064553302234595178&rtpof=true&sd=true">Request with an invalid value for the "invite code" key</a><br><br>

<h5><strong>Bug reports</strong></h5>
- <a href="https://docs.google.com/spreadsheets/d/1yyTTQz5-Sj18Bj5u6iT-W3JxO7q80B_doJE2B71GNdA/edit?usp=drive_link">JSON data in the response body isn't matched with the technical task after sending the argument with an invalid value for the "name" key.</a><br>
- <a href="https://docs.google.com/spreadsheets/d/1naco2jsyGZx9750tzzymmdFa2raWN0kwfsmNIvClzOY/edit?usp=drive_link">JSON data in the response body isn't matched with the technical task after sending invalid data in the "inviteCode" key.</a><br>
- <a href="https://docs.google.com/spreadsheets/d/1GUh7iq5HOQi4Y1UEAvH2Tiz7EjniMKI_TgmAdWLBZxA/edit#gid=0">JSON data in the response body isn't matched with the technical task after when one invite code is used more than 5 times.</a>

