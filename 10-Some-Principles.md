# Some Principles

- The core of RSS’ success is its simplicity. Necessarily, as we try
  to extend RSS to support a new menagerie of information, extra
  complexity will be introduced. But we mean to introduce that
  complexity incrementally and in layers.
   - As the RSS specification
     [describes](https://www.rssboard.org/rss-specification#extendingRss),
     new functionality will be specified in separate RSS
     namespaces. Clients can ignore those extensions or, hopefully,
     come to support them over time.
   - Each extension will bring new possibilities and functionality,
     but clients can pick and choose which to support and which to
     ignore at any given time. Whatever extensions they support will
     confer new features. Clients choice not to support a given
     extension won’t break anything. The core RSS tags, and core RSS
     functionality, will always work, and would render passably in an
     RSS client from 2009.
- Drawing from the experience of podcasts, extended RSS feeds can be
  the logical core of a wide variety of applications. In
  contradistinction to the internet of 2003 when *websites* were
  primary and RSS feeds were metadata or indexes of those sites, in
  2024 we hope to experiment with RSS feeds *as* the site or
  application, which a wide variety of RSS clients might render, and
  which can include as metadata references to online service that can
  render the feed and its item for users accessing applications
  directly from a web browser.
- As much as possible, we hope to build on top of primitives that are
  already widely accessible to web developers. As a namespaced
  extension, RSS documents will contain metadata, which might indicate
  that they represent a source that may be acted upon as well as
  merely read. Those actions will be specified as HTTP POST / PUT /
  DELETE etc, ordinary for web developers to work with. Identity
  (*qua* BlueSky) will be piggy-backed on top of simple DNS.
