# Introduction

Before social media, the internet itself was the social
platform.

Humans posted communications to websites on disparate
servers. Interested humans read those communications, and then
replied, sometimes by virtue of facilities offered by the website to
which they were replying, sometimes simply by posting a new
communication on some other web server.

Posting and reading across disparate websites was a very ethical
model, because the network itself is fundamentally public. The network
exists to create network effects, the social value that grows as more
and more people can communicate and interact and transact with one
another.

On deontological grounds, economic grounds, as well as
democratic and philosophical grounds, it is desirable that network
effects accrue to the broad public rather than be captured and
enclosed by a few firms or “platforms”:

- Every participant of the network contributes to network value, so
  all participants should have a claim to a share of value, and
  meaningful control over their own use of the network.
- Privatization of network value creates structural advantages that
  concentrate benefits and foreclose meaningful competition,
  destroying the foundation of a free-enterprise economy while its
  winners parade as false idols of free-enterprise success.
- How we communicate structures who we are as a polity; a polity
  committed to equal dignity should be made of coequal participants
  who share roughly equally in the opportunities engendered by the
  networks that bind us.

This is the vision that tacitly, or perhaps serendipitously, shaped
the early days of the internet.

There were, and are, pragmatic barriers to realizing this vision. If
the humans will post in disparate places, how will they be notified those
new communications even exist? When humans respond by posting in
“their own” corner of the internet, how do the authors of the original
post learn of and track the evolving discussion?

Around the turn of the millennium, 
[Dave Winer, Ramanathan Guha, and Dan Libby](https://www.rssboard.org/rss-history) 
offered a simple and
elegant solution to the discoverability problem. Websites would be
accompanied by machine readable summaries of their postings in a
format called RSS. These summaries would be updated whenever a new
item became available. Automated user agents —“RSS clients” — could
periodically poll these documents, and notify users whenever a new
posting appears on a source to which the user had “subscribed”.

Since these per-source summaries would be ubiquitous, and the
internet’s primary medium was hypertext, simply by following links
humans could quickly sample communities of interest and subscribe to
what they offer. As time passes and conversations occur, more links
and more sources present themselves. RSS clients offered a wide
variety of tools — very concise “headline”-style layouts, “folders”
into which related feeds could be collapsed, filtering by keyword,
etc. — to help users manage large collections of monitored sources.

RSS was a huge success. From about the year 2000 until the early
2010s, the internet itself was a thriving social network, replete
with high quality work of every variety posted in widely disparate
places, but discoverable and accessible to all through RSS readers.

Unfortunately, RSS and its “feed reader” clients alone did not provide
all of what users desired in order to collaborate and communicate
easily with one another. While various protocols
[were](https://en.wikipedia.org/wiki/Pingback)
[devised](https://en.wikipedia.org/wiki/Webmention) to notify authors
when new posts elsewhere respond to their work, these protocols were
more complex and less ubiquitously deployed than RSS, and succeeded
only partially.

RSS did not address an even more foundational problem: How do posts,
along with their accompanying RSS summaries, find their way onto the
internet in the first place? Initially the internet was populated by
academics and “geeks”, who were willing to overcome a variety of set-up
costs. As the ‘net grew ubiquitous, nearly everyone hoped to
participate, posting baby pictures or jokes or quick comments on
current events or restaurant reviews.

The demand for widely accessible, zero-friction posting, notification,
and discoverability created an opportunity for entrepreneurs
concerned more with profit than any ethical attachment to an open public
internet. They could draw users into “platforms” or “walled gardens”, and then "monetize" them. 
By the
early 2020s, the result of these “innovations” was an anti-ethical
internet, a site of corporate concentration and monopoly, describing a
polity of influence games rather than participation and deliberation
on terms equal to all.

RSS stands for “Really Simple Syndication”. Here in the 2020s, most
users think of RSS and “Google Reader” as also-rans, retro or
yesterday’s technologies, if they know of RSS at all. It stands as a
testament to the quality of RSS’ design, however, that behind the
scenes RSS remains widely adopted. It is simple &mdash; extraordinarily
simple, in economic terms cheap &mdash; to implement. You might as well
accompany your website with an RSS feed. Further, the one major
internet application that has evaded enclosure into platforms —
podcasting — has RSS at its core. Indeed, podcasts are little more
than RSS files accompanying sound files.

Whether by foresight or serendipity, RSS’ originators crafted a
protocol replete with imperfections, but resilient by
virtue of the simplicity of its foundation, and the ease with which
that foundation can be extended while fully preserving its core
functionality. Contemporary podcasts include extensions authored by
Apple, and also often by Spotify and Google, with annotations from
erstwhile RSS rival atom. RSS clients — including every podcast app! —
look for the extensions they know how to handle, which can enrich the
user experience and enable dramatic new functions. But they can fall
back to the old RSS core, ignoring whatever bells and whistles they
don’t understand, and do a serviceable job of notifying users and
making available new work.

In these dark ages, people are experimenting with a wide variety of
technologies to try to recover an open, public internet, where value,
control, and opportunity are widely dispersed and widely
shared. [ActivityPub](https://activitypub.rocks/), for example,
represents a notable public protocol intended to reproduce the
features that drew the public towards private platforms but under an
open and federated infrastructure. Blockchain projects, at their best,
hope to create open public platforms for applications that require
very high integrity or that involve transfers of financial
value. Beyond blockchains, cryptographically-inspired protocols like
IPFS offer new forms of decentralized, censorship-resistant, public
spaces on the internet. All of these represent interesting approaches.

But they are not simple.

RSS remains as simple as it was in 2003. RSS is accessible to
developers of ordinary talent and education without requiring months
of study to really get up to speed. RSS remains as straightforwardly
extensible as it ever was.

And the space that RSS *could* fill remains, oddly, almost entirely
unexplored. When Facebook — and Twitter and Google — moved fast and
broke things, they seduced the public from the open-internet with its
sinews of RSS so quickly and so definitively that we collectively
entered a brave new world. Except for podcasting, RSS fell into a
kind of stasis. A decade later, a discontented world is trying fancy
new things.

But it is our contention that much of what we want from an open
internet, one more broadly accessible and participatory than the
internet of 2010, can be provided with simple RSS. By simply extending
RSS precisely in the way it was designed to be extended, by addressing
entities that are logically RSS feeds with HTTP beyond the simple GET
methods, by using DNS to ensure that feeds and collections of feeds
can belong portably to their authors and owners, we can do a lot
better than Facebook and Twitter, and a lot better than old-school
blogs with comment sections, which themselves were walled gardens
under a feudal lord.

We can build a much better future simply by going back and RSS-ing all
the things.
