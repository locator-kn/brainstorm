
## possible plugins to use
* simplesmpt
* **nodemailer**
* **nodemailer-html-to-text**
* nodemailer-markdown

## possible uses
* **registration mail**
* newsletter
* notification if new trips available
* first contact message for trip - after timeout of ~30min 
* new chat message received - after timeout of ~30min
* notification setup for user -> disable notifications
* email or pwd forgotten

## admin page to handle emails
### configurations
* templates
* mail history
* timeout
* mail message
  * from
  * subject
  * text
  * ...
* SMTP setup

### functions
* send mail to all user
* send mail to specific user
* create templates
* load templates
* edit templates
* add attachment

### other stuff to check
* seccurity
* mail addr
* Server
* 

####GET

|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/mail/registration/:userid  | send mail to confirm registration | json object | statusCode: 404 |
|/mail/forgotten/password/:userid  | send mail to generate new password for user 'uderid'   | json object | statusCode: 404 |


### Dummy Json
```
{
   "_id": "ed5ad22e5fc3cb76148be1935f3f0f43",
   "_rev": "1-1e1d43f3df9b888fe9fa18cdcab45864",
   "title": "Complete Registration on locator-app.de",
   "linktext": "Click here to complete your registration on locator-app.de",
   "bodytext": "You recently signed up for locator. Please confirm your email address to get started!",
   "type": "registration_mail"
}
 

```
