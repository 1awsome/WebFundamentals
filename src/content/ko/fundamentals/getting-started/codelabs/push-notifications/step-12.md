project_path: /web/_project.yaml
book_path: /web/fundamentals/_book.yaml
description: Congratulations! You built a web app that enables Push Notifications.

{# wf_review_required #}
{# wf_updated_on: 2015-09-27 #}
{# wf_published_on: 2000-01-01 #}

# Congratulations {: .page-title }

{% include "_shared/contributors/TODO.html" %}




Pat yourself on the back. You built a web app that enables Push Notifications!

<div class="wf-highlight-list wf-highlight-list--learning">
  <h3 class="wf-highlight-list__title">Note</h3>
  <ul class="wf-highlight-list__list">
    <li>
      Be sure to check out 
      <a href="/web/fundamentals/engage-and-retain/push-notifications/">
      Push Notification</a> for best practices and more details on how to use
      Web Push Notifications.
    </li>
  </ul>
</div>

### Frequently Asked Questions

* **My service worker didn't update!**<br>
Are you sure? Check the source tab in _chrome://serviceworker-internals_. If it
really didn't update, restart Chrome.

* **I tried everything, but my service worker's still not updating :^|**<br>
Did you check and validate your code? If your service worker code can't be
parsed, it won't install.

* **My request to GCM is failing**<br>
Check the project on [console.developers.google.com](https://console.developers.google.com/). Make sure that the _gcm\_sender\_id_ matches the Project Number and the Authorization
key value matches the API key. Make sure you're looking at the right project!

* **The request to GCM is working, but no push event is fired**<br>
Check the subscription ID from the console for _main.js_. Is the subscription
ID in the array of IDs for your request correctly? Make sure you you have the
messaging API enabled on
[console.developers.google.com](https://console.developers.google.com/).

* **I'm getting errors I don't understand**<br>
Try using Chrome Canary: this often gives more informative error messages about
service worker woes.

* **I'm not seeing console logs for events in my service worker**<br>
You'll only get installed and activated events the first time you use the
service worker or when the code is changed. The started event will only be fired
once for each service worker session.

* **What about Firefox?**<br>
[As of Firefox
42](https://groups.google.com/forum/#!topic/mozilla.dev.platform/BL6TrHN73dY) the Push API is turned on by default.

### What we've covered

* Install a service worker and handle events
* Set up a Google Cloud Messaging (GCM) account
* Add a web manifest
* Enable a service worker to handle push message events
* Send a request to GCM via cURL or XHR
* Display notifications
* Handle notification clicks

### Next Steps

* Service worker codelab (if you haven't already done it!)

### Dive Deeper

* [Web Push Notification Documentation](/web/fundamentals/engage-and-retain/push-notifications/)
* [Using VAPID and the Web Push Protocol](/web/updates/2016/07/web-push-interop-wins)
* [Google Cloud Messaging Documentation](https://developers.google.com/cloud-messaging/)
* [Android Material Design Notifications Guidelines](https://www.google.com/design/spec/patterns/notifications.html)
