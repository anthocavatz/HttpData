HttpData
========

Utility for HttpRequest execution on Android

Requirement
-----------

* apache httpclient
* apache httpmime

Usage
-----

Very simply to use !

Execute GET request on URL and retreview result as String:
* String html = new HttpData(url).get().asString();

Execute POST with date and retreview result as JSONObject:
* JSONObject json = new HttpData("http://dns.com/api.php").data("login", "email@mail.com").post().asJSONObject();

And you can manage cookies, known response status, ...
