# E-Mail Tracker Blocker

A lot of companies and mail services put little invisible images into their mails that contain a personalized url. Whenever you open their mail, this image is loaded from the server and the company knows that __you__ opened their mail.

```` html
    <img src="http://tracker.com/trk?yourid=<some_random_string>" 
         width="1" 
         height="1" 
         style="display:none !important;" 
         alt="">
````

This is how they know that their spam has reached you -- a good start to send more.


## How can I prevent this?

There are tools that show you, where programs want to connect, for example [Little Snitch](https://www.obdev.at/products/littlesnitch/index.html). This is great to discover a new url that is not on the list yet. 

The easiest and free way to block tracking is however [adding the urls to your `hosts` file](http://www.howtogeek.com/howto/27350/beginner-geek-how-to-edit-your-hosts-file/). This makes your system re-route the tracking-links into nirvana.

If you find new urls, create a pull request or an issue to add them to the list.

````
0.0.0.0   track.mixmax.com
0.0.0.0   securepubads.g.doubleclick.net
0.0.0.0   click.mailer.atlassian.com
0.0.0.0   marketing.intercom-mail-200.com 
0.0.0.0   mailchimp.com
0.0.0.0   list-manage.com
0.0.0.0   cl.exct.net
0.0.0.0   emailtracking.azure.com
0.0.0.0   trker1.azalead.com
0.0.0.0   mkto-k0023.com
0.0.0.0   maileon.com
0.0.0.0   xqueue.de
0.0.0.0   t.yesware.com
0.0.0.0   track.getsidekick.com
0.0.0.0   t.sigopn01.com
0.0.0.0   t.senaluno.com
0.0.0.0   t.senaldos.com
0.0.0.0   t.senaltres.com
0.0.0.0   t.senalquatro.com
0.0.0.0   t.senalcinco.com
0.0.0.0   t.sigopn02.com
0.0.0.0   t.sigopn03.com
0.0.0.0   t.sigopn04.com
0.0.0.0   t.sigopn05.com
0.0.0.0   t.signauxun.com
0.0.0.0   t.signauxdeux.com
0.0.0.0   t.signauxtrois.com
0.0.0.0   t.signauxquatre.com
0.0.0.0   t.signauxcinq.com
0.0.0.0   t.signauxsix.com
0.0.0.0   t.signauxsept.com
0.0.0.0   t.signauxhuit.com
0.0.0.0   t.signauxdix.com
0.0.0.0   t.signauxneuf.com
0.0.0.0   t.signaleuna.com
0.0.0.0   t.signaledue.com
0.0.0.0   t.signaletre.com
0.0.0.0   t.signalequattro.com
0.0.0.0   t.signalecinque.com
0.0.0.0   t.strk01.email
0.0.0.0   t.strk02.email
0.0.0.0   t.strk03.email
0.0.0.0   t.strk04.email
0.0.0.0   t.strk05.email
0.0.0.0   t.strk06.email
0.0.0.0   t.strk07.email
0.0.0.0   t.strk08.email
0.0.0.0   t.strk09.email
0.0.0.0   t.strk10.email
0.0.0.0   t.strk11.email
0.0.0.0   t.strk12.email
0.0.0.0   t.strk13.email
0.0.0.0   t.sidekickopen01.com
0.0.0.0   t.sidekickopen02.com
0.0.0.0   t.sidekickopen03.com
0.0.0.0   t.sidekickopen04.com
0.0.0.0   t.sidekickopen05.com
0.0.0.0   t.sidekickopen06.com
0.0.0.0   t.sidekickopen07.com
0.0.0.0   t.sidekickopen08.com
0.0.0.0   t.sidekickopen09.com
0.0.0.0   t.sidekickopen10.com
0.0.0.0   t.sidekickopen11.com
0.0.0.0   t.sidekickopen12.com
0.0.0.0   mailtrack.io
0.0.0.0   mailstat.us
0.0.0.0   go.toutapp.com
0.0.0.0   app.outreach.io
0.0.0.0   tracking.cirrusinsight.com
0.0.0.0   app.yesware.com
0.0.0.0   t.yesware.com
0.0.0.0   mailfoogae.appspot.com
0.0.0.0   launchbit.com
0.0.0.0   cmail1.com
0.0.0.0   infusionsoft.com
0.0.0.0   via.intercom.io
0.0.0.0   mandrillapp.com
0.0.0.0   t.hsms06.com
0.0.0.0   app.relateiq.com
0.0.0.0   go.rjmetrics.com
0.0.0.0   web.frontapp.com
0.0.0.0   sendgrid.net
0.0.0.0   icptrack.com
0.0.0.0   click.icptrack.com
0.0.0.0   bl-1.com
0.0.0.0   links.mixmax.com
0.0.0.0   app.mixmax.com
0.0.0.0   ping.answerbook.com
0.0.0.0   constantcontact.com
0.0.0.0   google-analytics.com
0.0.0.0   mkt4477.com
0.0.0.0   api.mixpanel.com
0.0.0.0   mixpanel.com
0.0.0.0   list-manage.com
0.0.0.0   list-manage1.com
0.0.0.0   ihrgeld2016.com
0.0.0.0   doubleclick.net
0.0.0.0   webtrekk.net
0.0.0.0   elaine-asp.de
0.0.0.0   pstmrk.it
````


## Who would DO this?!

There are a lot of e-mail tracking tools online, for example:
- Mystrika https://mystrika.com
- Yesware http://www.yesware.com
- MailChimp http://www.mailchimp.com
- Sidekick by Hubspot https://app.getsidekick.com
- ToutApp https://www1.toutapp.com
- Streak https://www.streak.com
- ContactMonkey http://www.contactmonkey.com
- MailTrack https://mailtrack.io
- SalesHandy https://www.saleshandy.com
- Maileon http://maileon.com & https://www.xqueue.de


## How can I help?

If you get an e-mail by someone who might have an interest in wheter you read it (i.e. marketing-people, companies, shops), look at the source (*) and try to find something like the above code. It is usually at the very end of the mail. [Create an issue](https://github.com/JannikArndt/EMailTrackerBlocker/issues/new) with the url and I'll add it to the list!

### How can I see the e-mail source?

- macOS Mail: `View` > `Message` > `Raw Source`
- Outlook: Right-click anywhere in the message and select `View Source`
- Thunderbird: Select `View` > `Message Source` (or hit `Ctrl+U`)
- GMail: Open message > Click on the down arrow next to the reply arrow > `Show original`
