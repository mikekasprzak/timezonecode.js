# TimeZoneCode.js
The Problem: Web Browsers don't use internal names of timezones that people understand. You can get the UTC offset everywhere, but if you're in Canada or the US, you're used to codes like EST, EDT, PST, PDT, etc.

This is a project that began with Ludum Dare. We tried to create a system where a person visiting our website could instinctively read our clocks, and know exactly when our event would start. Alas, our method of trying to reverse-engineer timezones from the data emitted by the browser wasn't fruitful. It mostly worked, but there are a lot of minor cases we could solve if we made some assumptions given the language and UTC code.


