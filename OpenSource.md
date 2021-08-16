# Open Source Contributions
## [Statfink](https://sourceforge.net/projects/statfink/) [2006-2010]
Statfink is a php based live stat tracker for Yahoo-based fantasy football leagues.  Although this has been a free feature for years now, there was a time when it was a paid upgrade.  After discovering the project in my search for a way to track live score updates for a league I had recently created, I started playing around with the code to improve some of the functionality, and eventually contacted the project creator and became a primary contributor, ultimately contributing several significant enhancements on a project that saw 14k downloads per month at it's height of popularity.   Although this wasn't a professional endeavor, it was my first step into the world of open source!
### Contributions
- numerous _(search the [changelog](http://svn.code.sf.net/p/statfink/code/trunk/statfink/changelog.txt) for bsakc)_ 

<br>

## [IANA (Olson) Time Zone Database](https://www.iana.org/time-zones) [2019]
The [tz database](https://en.wikipedia.org/wiki/Tz_database) (also known as IANA Timezone Database or Olson database) is a collaborative compilation of information about the world's time zones, on which numerous computer programs and operating systems rely.

### Contributions
-  [Fix historical dst bug](https://github.com/eggert/tz/commit/38c2ee9acc0b6d3bd1e70bc7caee934ad75f147d) [06/2019]

   In the spring of 2019, [Brazil announced that it would be abolishing daylight savings time permanently](https://www.business-standard.com/article/news-ians/bolsonaro-ends-daylight-savings-time-in-brazil-119042600163_1.html).  This meant that we would need to deliver a patch to the tz database for our Brazil clients.  Because the change had to be delivered in short order, and on a code base shared by our much larger North America client base, we needed to ensure that the change would have no unintended consequences.  Because of this, as part of preparation for the upgrade, I wrote a suite of tests that ran against both the 2019a and 2019b versions of the database to catch any un-intended timezone rule changes.  As part of this suite of tests, I discovered a bug that was introduced around some historical DST rules.  While the changes wouldn't have affected us, I nonetheless submitted a patch and [the bug was fixed](https://github.com/eggert/tz/commit/38c2ee9acc0b6d3bd1e70bc7caee934ad75f147d). 

<br>

## [Joda-Time](https://www.joda.org/joda-time/) [2019]
The standard date and time classes prior to Java SE 8 are poor. By tackling this problem head-on, Joda-Time became the de facto standard date and time library for Java prior to Java SE 8.

### Contributions

- [Merged 2019b TimeZone database updates](https://github.com/JodaOrg/joda-time/pull/510) [06/2019] 

<br>

## [Troposphere](https://github.com/cloudtools/troposphere) [2020]
Troposphere is a python library that allows for easier creation of the AWS CloudFormation JSON by writing Python code to describe the AWS resources.

### Contributions

- [Fix FailOnWarnings data type](https://github.com/cloudtools/troposphere/pull/1656) [04/2020]  

<br>

## [airflow-helm](https://artifacthub.io/packages/helm/airflow-helm/airflow) [2021]
Community-maintained helm chart for Apache Airflow.  This chart pre-dated the "official" apache chart and is used by thousands of companies for their production deployments of Airflow.

### Contributions

- [ensure git-sync is the first init-container](https://github.com/airflow-helm/charts/pull/307) [07/2021]

<br>

## [Apache Airflow](https://airflow.apache.org/) [2021]

### Contributions

- [open relative links in place](https://github.com/apache/airflow/pull/17477) [08/2021]


