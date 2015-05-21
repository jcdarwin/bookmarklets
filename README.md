# What is this?

This is a list of useful bookmarklets.

Drag the link your're interested in to you browser bookmarks bar.

## Bookmarklet to listen for an event
This bookmarklet will report a message to the browser console when it sees a particular event (requires jQuery to be loaded on the page).

### The code:
(function() {
    if (jQuery) {
        jQuery(document).bind('analytics', function(e){
            // Do something as a consequence of receiving the event
            console.log('I just saw an "analytics event: "', e);
        });
    }
})()

### The link:
[Drag me to the browser bookmarks bar](javascript:void%20function(){jQuery%26%26jQuery(document).bind(%22analytics%22,function(n){console.log('I%20just%20saw%20an%20%22analytics%20event:%20%22',n)})}();)
