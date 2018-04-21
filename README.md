# TimeZoneCode.js
The Problem: Web Browsers don't use internal names of timezones that people understand. You can get the UTC offset everywhere, but if you're in Canada or the US, you're used to codes like EST, EDT, PST, PDT, etc.

This is a project that began with Ludum Dare. We tried to create a system where a person visiting our website could instinctively read our clocks, and know exactly when our event would start. Alas, our method of trying to reverse-engineer timezones from the data emitted by the browser wasn't fruitful. It mostly worked, but there are a lot of minor cases we could solve if we made some assumptions given the language and UTC code.

The chosen names are user vetted. We tried to pick names that a local user in their home timezone would understand.

TimeZoneCode.js uses English names by default, but it can optionally use a localized name where available (but only your own timezones). For example, you will not get Eastern Standard Time (EST) localized in to German, but Central European Time (CET) in Germany can optionally be Mitteleuropäische Zeit (MEZ).
