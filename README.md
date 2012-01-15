An Unofficial So.cl Google Chrome Extension API
================================================

What is it about:
----

I provide you a very basic asynchronous So.cl API, in the current
release, you can do the following:

- Count/List/Clear your notifications


How does it work?
----

Microsoft signs all the requests with HMAC id that gets calculated. So this
API does adds stuff to the $.ajax prefilter so that it can amend the timestamp
and signed key. It uses a HMA SHA256 Base 64 signature. Thanks to Google Crypto
API, we got the signature to sign each AJAX request.

The signed key and time are *always* needed or it will explicitly return back that
your not authenticated.

Contributions welcomed!
----

If you would like to continue adding methods, please fork and submit a pull request.
At this time it is pretty easy adding more API methods, you just inspect each request
and analyse!

Thanks,
Mohamed Mansour