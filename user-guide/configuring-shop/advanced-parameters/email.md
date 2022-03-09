# Email

Your shop sends many messages throughout all the steps of registration and placing an order. Here, you can configure how these messages will be sent, and see what messages were sent.

## E-mail <a href="#email-e-mail" id="email-e-mail"></a>

The first section of the page presents you with a list of all the emails that were sent from PrestaShop, with the recipient, the template used, the language of the message, the subject of the email and the time of sending.

![](<../../../.gitbook/assets/38469764 (4) (4) (3).png>)

## Email <a href="#email-email" id="email-email"></a>

This is where you decide how your emails are sent and received.

The form has three sets of options:

![](<../../../.gitbook/assets/38469765 (4) (4) (3).png>)

* **Send email to**. This is a front-end setting. At the end of the checkout process, a client can leave a message to your staff. You can choose to whom this message will be sent by selecting from the drop-down list. To add more addresses, you should go to Shop Parameters > Contacts.
* Email parameters: how emails are technically sent. Choose among the three. See below for more information.
* Email format: how email are visually sent. Choose among the three. See below for more information.
* **Log Emails**. Disable if you no longer want to keep track of the emails sent by your shop, as shown in the Email section above.

### Technical configuration <a href="#email-technicalconfiguration" id="email-technicalconfiguration"></a>

Configure PrestaShop to send emails to your customers. We strongly advise you that you consult your web host to determine which settings to use for this feature. The options are:

* **Never send e-mails**. Keep this setting for testing purpose. Once your shop is public, you should never use this setting.
* **Use PHP's mail() function**. This option is recommended by default. In the event that this does not work, then use the SMPT option below.
* **Set my own SMTP parameters**. In this case, a new section appears, with more fields. The information for these fields should be provided by your web host: mail domain name, SMTP server, SMTP user, etc. Make sure to transcribe exactly what your web host provides you with.

The SMTP configuration information can be provided to you either by:

* Your system administrator,
* Your host,
* Your ISP,
* Your e-mail provider.

![](<../../../.gitbook/assets/23789857 (4) (4) (3).png>)

Your web host can tell you whether or not your username is mandatory, as well as the password information, and the encryption to use.

For example, in the case of Gmail (the email service offered by Google), you might have to enter information such as the following one:

* SMTP server: [smtp.gmail.com](http://smtp.gmail.com)
* User: [my.user.name@gmail.com](mailto:my.user.name@gmail.com) (example)
* Password: RT22UE87 (example)
* Encryption: SSL
* Port: 465

### Visual configuration <a href="#email-visualconfiguration" id="email-visualconfiguration"></a>

There are two formats available for e-mails: HTML is great to look at, but might not work everywhere; text is dull to look at, but works everywhere.

You can choose to use only one of the two, or both. Both is the recommended way.

## Test your email configuration <a href="#email-testyouremailconfiguration" id="email-testyouremailconfiguration"></a>

Once you have configured your emails using one of the two available methods, enter your own e-mail address in this section, then click the "Send a test email" button.\
Now check the inbox of the address provided to verify that you indeed have received the test email, in the correct format. If you have not received it, update your configuration with the correct information.

![](<../../../.gitbook/assets/38469768 (4) (4) (3).png>)
