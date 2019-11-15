# W2E: A Worldwide-Event Benchmark Dataset for Topic Detection and Tracking
**Reference**: Tuan-Anh Hoang, Khoi Duy Vo, and Wolfgang Nejdl. 2018. W2E: A Worldwide-Event Benchmark Dataset for Topic Detection and Tracking. In Proceedings of the 27th ACM International Conference on Information and Knowledge Management (CIKM '18). ACM, New York, NY, USA, 1847-1850.([pdf](https://www.dropbox.com/s/r1cmuiu6fyw6zsf/w2e.pdf?dl=0))

# Events
This [file](https://www.dropbox.com/s/npqie5hxcy24o1v/events_grouped_by_topic_with_manually_constructed_queries.csv?dl=0) contains all events together with its (original-unmerged) topic as extracted from Wikipedia Current Events portal in 2016. Each topic has one line containing the the topic's information (4 tab-separated fields: ID, category, a '****' string, and the description), follows by Nx2 lines for its N events. Each event has 2 lines: the first line contains the event's information (2 tab-separated fields: date of the event, and the event's summary), the second line contains the search query that is manually constructed for the event.

Example: 
"
TOPIC-7	Disasters and accidents	***	Kollam temple fire
2016-04-10	A fire occurs at a Hindu temple in the Kollam district ...
Kollam Kerala India Hindu temple fire
2016-04-11	Five workers from the company that supplied fireworks to the Puttingal Temple ...
worker fireworks Puttingal Temple dead
"
means TOPIC-7 belong to "Disasters and accidents" category and the description is "Disasters and accidents". This topic has 2 events, happening on 2016-04-10 and 2016-04-11 respectively. The two queries for those events are Kollam Kerala India Hindu temple fire and worker fireworks Puttingal Temple dead respectively.

# Merged Topics
This [file](https://www.dropbox.com/s/rewjqzxipbntezp/topicGroups.txt?dl=0) contains all topics merged together in to bigger topics - here called GROUP. Each group is denoted by group ID and follows by the set of its topics. Events of group's topic member are also listed.

Example:
"
GROUP-3
TOPIC-1386	Politics and elections	South Korea's opposition holds ...
2016-02-24	South Korea's opposition holds a parliamentary filibuster, ...
TOPIC-2678	Politics and elections	South Korean opposition lawmakers' anti-terrorism bill ...
2016-02-28	South Korean opposition lawmakers' anti-terrorism bill filibuster...
"
means TOPIC-1386 and TOPIC-2678 are merged together under GROUP-3. Each of the two topics has one event that happens on 2016-02-24 and 2016-02-28 respectively.

# News Agencies
This [file](https://www.dropbox.com/s/uimfmxyx1m3qamj/agencies.txt?dl=0) contains the list of all the news agencies where we collected articles from.

# Articles

This [file](https://www.dropbox.com/s/mi0dpk15cta95r6/topics.zip?dl=0) contains all URLs to articles that are manually judged relevant to the events.  For the articles' content, please write to hoang_at_l3s_dot_de
