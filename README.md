localstars
==========

via (store.js)[https://github.com/marcuswestin/store.js/] uses HTML5 localstorage to keep
track of what pages are stored in a local list of "starred" or favorited pages on the
current website.

due to the (same origin policy)[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Same_origin_policy_for_JavaScript]
the fact that a page has been "localstarred" can be known to any
javascript running on any page served from the the same `hostname:port`.

The key used in the local store starts with the sting `localstars.`
and ends with the value of `window.location.pathname`.  Right now, only
"True" is stored in localstorage; but an associative array of citation metadata 
could be stored in there.


