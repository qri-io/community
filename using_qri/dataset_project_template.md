# Dataset Project Template

Qri doesn't work without data you care about. This project template is the high-level workflow we use to understand the process of creating meaninful data. While working with Qri others will often ask what you goal is, what sources you've considered, and where they can find your results. This template is one way to think about that workflow

** **

### 1. Define a goal
Pick something you want to learn more about. At this phase it's important to _not_ think just about data, but instead about _what you want to learn_. The "data" part will come naturally, but it's important to try your best to define _what_ you want to know and _why_ you think it would help to know that thing.

There's a very good chance you'll come back & adjust your goal after doing some research

_example:_ 
> goal: Understand how the epa.gov sitemap changes over time.
> motivation: How often pages are linked to is an indicator of what content is being emphasized. There are many other indicators. This one is quantative, and can be collected with the resources we have on hand.

### 2. Find & document sources
Find out what's out there. These might be data sources, these might be PDF's, these might be books in a library. What's important is to _assemble a list of sources_ as you go. This is the core of your research.

At this point, you might find the answer to your question outright. Maybe you found someone who's written a paper that answers your question, or an existing dataset already breaks down what you'd like to know in a way that's close enough. If that's the case, cite that work! Tell others that it answered a question for you, and know the research you've done to find that work is time well spent.

If you _don't_ find sufficient sources, you have options.
* **Keep looking for sources:** It can be hard to know when to move past the source-finding phase, but good data can show up in hard-to-find places. You may need to email folks, file a FOIA request, or head to the library. It's always worth asking if you've found enough sources, or the right source
* **Move on:** Sometimes the thing you want to learn is simply too difficult to turn into data. At this point it's worth either re-thinking your approach, or switching to a new subject of research. Either way, keep notes on your choice!
* **Build Something:** Often, you'll need to build a dataset to answer your question properly. At this point, it's time to move on to step 3.


_example:_
Places we've checked for sitemaps:
* Google: turns out they don't publish sitemaps
* ... (more research here)

An open source project called [walk](https://github.com/qri-io/walk) can generate sitemaps. Use that to build a sitemap of epa.gov. Create that dataset at a regular inverval (say, once a week).


### 3. Build & Analyze Dataset(s)
Draw from a selection of your sources to create & aggregate data in a way that produces an insight. Keep iterating until you've come to an initial result, then compare that result to your goal. Does this result answer the question you'd initially asked? It may be necessary to combine different sources from your list, gather new sources, and adjust your goals until you arrive at data that informs your goal.

Qri can help with this process in a number of ways, by generating versions of datasets while you work, and providing other supplemental datasets to integrate into your work.

_example:_
After creating two versions of a dataset, use Qri to create a derivative dataset describing the difference from version to version with high-level stats most useful for analysis:
* pages with the highest number of added links-to
* pages with the highest number of removed links-to
* pages who's link-to count has dropped to zero


### 4. Vizualize & Publish
Once you've _found_ an insight, the next thing to do is draw others to what you've found. Using Qri, the best way to do that is to present your findings is to build a visualization & publish it.

_example:_
Build a visualization that presents the date range, crawl settings, domain, and each of the three lists as top-200 overview lists for quick reference. Publish to app.qri.io so others can grab raw data


### 5. Automate
Finally, data often goes stale. Set up automation so that your dataset _updates itself_, allowing you & others to continually benefit from your work without needing your intervention.

_example:_
Schedule both sitemap dataset and sitemap analysis dataset for updates each week, with regular publishing.