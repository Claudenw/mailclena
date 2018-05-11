# mailclena
Tool that logs into mail accounts and removes all mails.

## Stats

[![Waffle.io - Columns and their card count](https://badge.waffle.io/ottlinger/mailclena.svg?columns=all)](https://waffle.io/ottlinger/mailclena)


[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/ottlinger/mailclena.svg)](http://isitmaintained.com/project/ottlinger/mailclena "Average time to resolve an issue")
[![Percentage of issues still open](http://isitmaintained.com/badge/open/ottlinger/mailclena.svg)](http://isitmaintained.com/project/ottlinger/mailclena "Percentage of issues still open")
[![Known Vulnerabilities](https://snyk.io/test/github/ottlinger/mailclena/badge.svg)](https://snyk.io/test/github/ottlinger/mailclena)
[![GPL v3.0](https://img.shields.io/github/license/ottlinger/mailclena.svg)](https://www.gnu.org/licenses/gpl-3.0.en.html)

## Github integrations
### Travis / CI

In order to just play around with it I've integrated a CI run:

[![Build Status](https://travis-ci.org/ottlinger/mailclena.svg?branch=master)](https://travis-ci.org/ottlinger/mailclena)

### Code coverage

[![codecov](https://codecov.io/gh/ottlinger/mailclena/branch/master/graph/badge.svg)](https://codecov.io/gh/ottlinger/mailclena)

### Codacy - code quality and static analysis

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/c8fc0c6ef3d14192a2a8f84a670ccb92)](https://www.codacy.com/app/github_25/mailclena)

## How to run and use the application

You need to checkout the application and build it with the help of [Java](https://java.sun.com) and [Maven](https://maven.apache.org/).

```
$ mvn
$ java -jar target/mailclena-0.0.1-SNAPSHOT-executable.jar
22:58:33.294 [main] INFO  de.aikiit.mailclena.MailClena - Hello World :-)
```

### Command line parameters

```
usage: MailClena
 -h,--host <arg>       Hostname - example: http://imap.yourisp.org
 -p,--password <arg>   Password - example: myfancypassword
 -u,--username <arg>   Username - example: myuser@tld.org

```

### Example call

```
$ java -jar target/mailclena-0.0.1-SNAPSHOT-executable.jar -h=host.tld.org -u=yourmail@yourtld.org -p=yourpassword

00:04:20.144 [main] INFO  de.aikiit.mailclena.MailClena - MailClena is launching with the given configuration ....
00:04:20.972 [main] INFO  de.aikiit.mailclena.mail.MailClient - Found 0 messages.
00:04:21.422 [main] INFO  de.aikiit.mailclena.mail.MailClient - Starting to delete 0 messages.
00:04:21.455 [main] INFO  de.aikiit.mailclena.mail.MailClient - Expunge folder to actually remove messages.
00:04:21.455 [main] INFO  de.aikiit.mailclena.mail.MailClient - Finished to delete 0 messages.
00:04:21.866 [main] INFO  de.aikiit.mailclena.mail.MailClient - Found 0 messages.
00:04:21.898 [main] INFO  de.aikiit.mailclena.MailClena - MailClena is shutting down .... bye bye :-)
```

## Project webpage

A Maven-generated site report is also available [here](https://ottlinger.github.io/mailclena/).
