---
title: "Welcome to Jekyll!"
date: 2017-10-20 08:26:28 -0400
categories: jekyll update
---
# test12345
드디어 블로그에 첫 글을 썼다.

```java
public static Logger setLog() {
		final Logger log = Logger.getLogger(Log.class);
		try {
			final String layout = "%d [%-15C{1}][%-5p] %m%n";
			// String layout = "%d %m%n";
			final String logfilename = "showdown.log";
			final String datePattern = ".yyyy-MM-dd";
			final PatternLayout patternlayout = new PatternLayout(layout);
			final DailyRollingFileAppender fileAppender = new DailyRollingFileAppender(patternlayout, logfilename,
					datePattern);

			log.addAppender(fileAppender);
			final ConsoleAppender consoleAppender = new ConsoleAppender(patternlayout);
			log.addAppender(consoleAppender);
			log.setLevel(Level.INFO);
		} catch (final Exception e) {
    }
    return log;
}
```