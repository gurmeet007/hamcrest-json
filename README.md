Hamcrest matchers for comparing JSON documents, backed by the [JSONassert library](https://github.com/skyscreamer/JSONassert).  The code is released under the [MIT license](http://www.opensource.org/licenses/mit-license.php).

Installation
============

To install from Maven Central:

```xml
<dependency>
	<groupId>uk.co.datumedge</groupId>
	<artifactId>hamcrest-json</artifactId>
	<version>0.1</version>
</dependency>
```

Usage
=====
```java
assertThat(
	"{\"age\":43, \"friend_ids\":[16, 52, 23]}",
	sameJSONAs("{\"friend_ids\":[52, 23, 16]}")
		.allowingExtraUnexpectedFields()
		.allowingAnyArrayOrdering());
```

Resources
=========
 * [hamcrest-json website](http://datumedge.co.uk/hamcrest-json/)
 * [API documentation](http://datumedge.co.uk/hamcrest-json/apidocs/index.html)