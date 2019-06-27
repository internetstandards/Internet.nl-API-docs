# Interactive e-mail test manual

This document describes the steps that need to be taken in order to perform the **interactive e-mail test**. Keep in mind that this the interactive e-mail test requires you to provide one e-mail address (a recipient) per domain.

## From the perspective of the API user

1. Inform the owners of the e-mail addresses used in the test that they can expect an e-mail from Internet.nl and ask them to follow the given instructions. You can use [this template](https://github.com/internetstandards/Internet.nl-API-docs/blob/master/interactive-mail-test-announcement.md) to inform them. 
2. Register a mail batch request using [our instructions](https://github.com/NLnetLabs/Internet.nl/blob/new_forumstandaardisatie_custom_view/documentation/batch_http_api.md) and make sure to add an e-mail address per domain using the same domain name.
3. The interactive e-mail test has a maximum running time of 3 days. That means that the recipient of the e-mail has 3 days time to respond to the e-mail. This is also mentioned in the e-mail the recipient is going to receive.

Notice:
* The result is available as soon as all replies have been recieved within the given time frame.
* If the receiver does not respond to the e-mail within the given time frame, only a few of the subtests as part of the interactive e-mail test will be performed.
* This test is only the interactive mail test; results from the normal mail test will not be included.
* E-mails recieved from recipients will to be saved with the results. They will be deleted after expiry of the given time frame.

## From the perspective of the recipient
1. An e-mail anouncing the interactive e-mail test is received from the API user ([template](https://github.com/internetstandards/Internet.nl-API-docs/blob/master/interactive-mail-test-announcement.md)).
2. After the API users has registered a mail batch request, the recipient recieves an e-mail with instructions coming from **@batch.internet.nl**. This e-mail will show the name and e-mail address of the API user to force ownership of the action and provide clarity for the recipient.
3. According to the instructions, the user needs to reply to the e-mail in order for the interactive e-mail test to continue.
4. When succesfully following the instructions, the recipient recieves a confirmation e-mail that his/her reply was received succesfully.

Notice:
* The results of the test will not be shared with the recipient. It's is up to the API user to inform the recipient.
