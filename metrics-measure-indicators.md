# Metrics, Measures, Indicators

Explanations:

* https://www.climate-eval.org/blog/whats-name-indicators-measures-and-metrics
* https://thecarebot.github.io/metrics-measures-and-indicators/


Having a shared understanding of what metrics are and what we mean by them helps teams focus on questioning the insights they take away from the data, rather than spending the time debating the definition and quality of the data they receive.

## Metrics

Metrics represent the different methods we employ to understand change over time across a number of dimensions or criteria. It is often used as a catch-all term to describe the method used to measure something, the resulting values obtained from measuring, as well as a calculated or combined set of measures.

We use the term measures when we mean the value measured by whatever mechanism we employ and the term indicator for values we combine and use to hint to specific outcomes and trends.

Note: All measures and indicators reflect events that occured in a specific period of time. When representing these values (specially when aggregating them), indicate the period of time it relates to.


## Measures

A measure is a number or a quantity that records a directly observable value or performance. All measures are composed of a value (a number) and a unit of measure. The number provides magnitude for the measure (how much), while the unit gives number meaning (what is measured).

* 1,234,567 Pageviews
* 8,901,234 Sessions
* 567,890 Facebook Likes


## Pitfalls with measures

When comparing measures that are tracked by two different systems (for example, the number of daily sessions on your site versus the number of daily sessions on your competitor’s site), ensure that the units are consistent between both. It is not uncommon for a measure of the same name to mean different things; consult the documentation that defines each measure for that system.

Even when the same system is used, there might still be differences. For example, a session in Google Analytics is defined as “A group of interactions that take place on a site within a given time frame.” It is set to expire after 30 minutes of innactivity by default, but this setting can be changed.

If, for example, you are comparing session length for stories with long-form video, you will likely adjust the default 30 minutes to a longer period to avoid timing out user sessions while they are still watching (but just paused and stepped away) and possibly miscounting the total number of sessions. If you do so, comparing sessions-related behaviors with another site that uses the 30 minute default may be a misleading comparison.


## Indicators

An indicator is a qualitative or quantitative factor or variable that provides a simple and reliable mean to express achievement, the attainment of a goal, or the results stemming from a specific change. It often aggregates or combines multiple measures in an explicit formula.

Examples:

* 1M weekly active users
* 1:3 users complete the story
* 23% homepage bounce rate


## Pitfalls with indicators

All indicators are relative to a set of measures in a particular context. For an indicator to be meaningful, it should always be contextualized with the scope of stories being assessed and the measures used to calculate should be made explicit.

It is very easy to get indicators wrong because they can obscure a lot of information and complexity with the deceivingly simple guise of a single value. Here are some situations:

### 1. Indicators are always relative to a context

“1:3 users complete the story” sounds as concrete and tangible as any other measure but the unit is not self-evident. There is no tangible “read-story” unit that can be tracked and counted. This abstraction forces introspection and requires a definitional understanding of all its parts.

What is a story? Is a text-based 2000-word page-scroll experience and an auto-advancing photo essay with an audio track both considered stories? Can they be compared? Should they be compared? *Are* they compared in this ‘1:3 users complete the story’ indicator?

While the answers may be yes, due to their inherent technical format difference they can’t actually be tracked in the same way. This is where the diversity of story forms in journalism makes analytics trickier than more simplistic ecommerce analytics, which are consistently transactional.

What measures are being used for each type? A video or audio piece may aggregate the total time played over media duration, whereas for an interactive graphic could take the total time the user spent viewing the graphic relative to an arbitrary ideal period of time. (These are other examples of items that may be considered “stories” in a specific context).


### 2. Indicators can be simplifying to a fault

Indicators obfuscate in order to clarify. By reliably providing just one method to observe change of a particular aspect over time and thus understand its performance (even if it is fairly complex or complicated), indicators help make the complex clear.

They accomplish this by obfuscating the details, rationales and definitions — in our example, the different ways in which it obtains the same metrics for different story forms, tracked by different means, and calculates a single number.

Obfuscating too much renders the indicator less clear because it hides some of that necessary context, which is so important to give meaning to the insight. Finding the right balance of offering useful insights while not overwhelming the user is a big challenge for meaningful analytics.


### 3. Indicators force value judgments

Numbers are agnostic. People attribute positive or negative meaning to numbers depending on the context in which they are used. Additionally, were averages, medians or total values of aggregated measures used? Each may give you a significantly different read on your data. This is further emphasized when indicators are presented in comparative terms such as relative to a specific goal or relative to existing benchmarks.

Bounce rate is an indicator used to describe the percentage of single-page sessions, meaning the sessions in which the person left the site from the same page they entered without interacting with the page. Is this good or bad? It can be bad if that page is the starting point of an interactive story and the expected next step was for the user to hit play and start navigating through the story. It is good if that was your contact page and people came to get your phone number or address.

Scrutinizing what the indicator means, what it attempts to represent, how it is calculated is a healthy way to uncover measurement ment problems.


