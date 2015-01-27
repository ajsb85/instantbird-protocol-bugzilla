# instantbird-protocol-bugzilla
Assists to setup a chat account for Bugzilla


http://www.bugzilla.org/ <br>
https://wiki.mozilla.org/Bugzilla:REST_API <br>
http://bugzilla.readthedocs.org/en/latest/api/index.html <br>
https://wiki.mozilla.org/BMO/ChangeNotificationSystem#Commands<br>
https://bugsnag.com/docs/notification-plugins <br>
https://mrcote.info/blog/2014/04/04/bugzfeed-bugzilla-push-notifications/ <br>
https://wiki.mozilla.org/Auto-tools/Projects/Pulse/Exchanges <br>
https://wiki.mozilla.org/BMO/ChangeNotificationSystem <br>
https://github.com/mozilla/bugzfeed <br>
http://people.mozilla.org/~mcote/bugzfeed_example/

## Examples of native REST API use
public data

Here are few examples of using the API (without logging in, so with public data)

Get all data for a single bug

https://bugzilla.mozilla.org/rest/bug/35 

However you almost always never need all data. Use "include_fields" to request just the data you need. Most of the calls to Bugzilla support "include_fields".

https://bugzilla.mozilla.org/rest/bug/35?include_fields=summary,status,resolution 

Get all comments for a single bug

https://bugzilla.mozilla.org/rest/bug/707428/comment 

Get history of all metadata changes for a single bug

https://bugzilla.mozilla.org/rest/bug/707428/history 

Get data for all the bugs in the 29 Branch

https://bugzilla.mozilla.org/rest/bug?version=29%20Branch 

Get data for all the bugs assigned to a particular user

https://bugzilla.mozilla.org/rest/bug?assigned_to=lhenry@mozilla.com 

Get data for all the bugs with the keyword "topcrash"

https://bugzilla.mozilla.org/rest/bug?keywords=topcrash 

Get all the bugs that are mentored

https://bugzilla.mozilla.org/rest/bug?product=Input&f1=bug_mentor&o1=isnotempty 

Get data about a particular product

https://bugzilla.mozilla.org/rest/product/firefox 

Get data about products and components

https://bugzilla.mozilla.org/rest/product/core?component=DOM 

Get data for a user

https://bugzilla.mozilla.org/rest/user?names=lhenry@mozilla.com 
