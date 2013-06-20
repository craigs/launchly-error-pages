launch.ly error pages
=====================

launch.ly Custom Error Pages Template

## How to make a custom 404 page in launch.ly

### Installation

Just create a snippet with the address pattern **ERROR** and copy in the contents of error-page.snippet. You can also add the styles from error-page.less to your theme style sets.

### Overview

By default, [launch.ly](http://launch.ly) has a bare bones internal error message snippet for when you hit a 4xx error. But all that says is something like "404. File not found". You probably would like to add a bit of style or even better, display something that might help the user end up in the right place. Things like a search box or a list of categories might be a great idea.

To override the default error page display, you will need to create an error page snippet. There is nothing special about this snippet except for the fact that the address pattern is set to "ERROR". You see, when launch.ly cannot find an item for a given link, it first looks to see if there is a snippet with the address pattern "ERROR" and displays that snippet if one exists, otherwise you will get the default internal message.

There are [heaps of error codes](http://en.wikipedia.org/wiki/List_of_HTTP_status_codes), and you have access to what the detected error code encountered was through the error_code variable. This way you can customise the messages based on the error code was encountered. I normally handle 404 messages and have a default page for all other error types.

The rest is up to you. Be creative.


### A little inspiration

OK, so here are some really great and creative 404 pages to inspire you.

- [lego.com](http://www.lego.com/file-not-found/)  
	lego.com have a great page. It features a single button linking back to the home page with a simple file not found message.
- [titleist.com](http://www.titleist.com/file-not-found/)  
	Being a golfing company, having a heap of golfers looking for a lost ball is a great analogy. They also include buttons linking to their major product sections.
- [github.com](https://github.com/file-not-found/)  
	github is a source code hosting platform which we use and love. In catering for nerds, a Star Wars reference is pretty obvious. But it features a search box to let you find other source repositories.
- [techcrunch.com](http://techcrunch.com/file-not-found/)  
	Tech Crunch has a wordy 404 page that links really well to a search page, but also asks you to report the error as well.
- [mashable.com](http://mashable.com/file-not-found/)  
	One big search box ... and a little humour.

### 404 Tracking and Correcting

If you have enabled Google Analytics on your account, 404 errors are automatically tagged as a custom event.

Visit google.com/analytics to check your 404 errors under Content > Events > Overview and you will see "Error" under the "Event Category" section. Drill down and see if you can fix any errors up by adding links to other items. If you have removed a product and it has been replaced by a new product, add the old links to your new item to solve the 404 errors. Your customers will love you for it.

### Don't forget, it's a great marketing opportunity.

Remember, your customer is looking at this page. I like to think of it as if someone walked in to your shop and didn't know where to go. You can either let them wander around and watch them walk out, of offer some help. Give them avenues to follow you on social media, and put some love in to it. I have even seen people use videos to great effect even inviting them in to the real store instead of being online.
Want to know how to make custom 404 error pages in launch.ly? I created a github project and posted an article at http://dev.launch.ly/blog/how-to-make-a-custom-404-page-in-launch-ly