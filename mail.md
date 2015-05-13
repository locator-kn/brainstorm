
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

### Dummy Json
```
{
   _id: 'asdf97a87dsf689as7d6fas87d',
   _rev: '1-dbe58c4eb46dc66b3b62ed4dfab2f3fe',
   title: 'Complete Registration on locator-app.de',
   linktext: 'Click here to complete your registration on locator-app.de',
   bodytext: 'You recently signed up for locator. Please confirm your email address to get started!',
   type: 'mail'
}
 

```
