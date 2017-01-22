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

## How to prevent this

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
0.0.0.0   mkto-k0023.com
````
