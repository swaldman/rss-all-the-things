# Project Outline

1. Recognize that a richly descriptive, client agnostic format
   embedding or linking core content should be the “canonical”
   description of on-line work, rather than html files which entangle
   a particular set of very contingent UI choices. Build on the
   simplicity and existing role of RSS, extended as it is designed to
   be extended, to serve as that format.
2. Define mix-or-match extensions to RSS that provide metadata across
   a variety of dimensions, so that these “canonical expressions” can
   be deployed, managed, aggregated, and presented in a wide variety
   of useful ways.

   “Dimensions” might include:
   - **An application dimension:** Podcasts, and Apple’s extensions of
     RSS to support them, are a touchstone example. Widely
     distributed, but aggregated and indexed, RSS-based content should
     be suitable to undergird a new commonwealth of letters (like the
     old blogosphere), microblogging and social media, and review
     applications (Yelp, Trip Advisor, GoodReads, Amazon product
     reviews, etc) while leaving ownership and control over content in
     widely dispersed hands. As with podcasts, feeds *can* include
     descriptions or recommendations of UI elements that rich,
     application-specific clients may choose to render while leaving
     the core data in basic (or near basic RSS), comprehensible to
     anything and everything.
   - **An attestation dimension:** It should be possible to attach
     digital signatures associated with identities to elements of RSS,
     in a context where the validity of the association between
     signing key and identity can be checked by clients and repudiated
     by identity owners in the event of compromise. [^1]
   - **A degree of curation dimension:** An RSS feed can represent
     everything from a single atomic “item” of content to a full
     listing of the source it represents. The degree of curation
     should be representable in machine-readable metadata. Dynamic
     services should provide information about the request or query
     that would have generated this curation and the source to which
     that request or query might be made, so that clients and users
     might vary or further refine those queries.
   - **A degree of completion dimension:** An RSS feed can signal
      1. as little as existence
         - a resource exists, here’s a link
      1. minimal metadata (title, authors, date) and optionally a
         short description or summary
      2. full content, by embedding or enclosure element
         - everything a rich client would require to fully represent
           the item, as long as it has access to the internet to
           collect linked subsidiary resources (images, etc.)
      1. complete embedding
         - the full content *and* subsidiary resources are fully
           embedded in the file. the file can serve as a stand-alone
           archive of the items it contains.

   When the degree of curation dimension is full-listing and the degree
   of completion element is complete-embedding, RSS can serve as a
   permanently readable backup and storage archive for collections of
   creative work.

3. Design and specify a kind of RSS service, which represents a
   dynamic repository of creative work and metadata representable as
   RSS feeds. Define standard (and very simple!) means of adding to,
   updating, querying, and archiving such repositories.
   - In such services, base feeds (as opposed to representations that
     are curations) should have owners and should be exportable as
     complete archival feeds. They should be transportable, as all
     links should be through owner-specific DNS names. Reimportation
     into a new service and redirection of DNS to that service
     migrates an author without breaking links.

[^1]: “PKI” — public key infrastructure — is in general a domain sorely in need of
protocol improvement. There exists an 
[XML signature](https://en.wikipedia.org/wiki/XML_Signature) standard
that could be deployed for attestations in RSS, but it is not
popular or straightforward among developers, and relying upon it
might tether RSS to aspects of XML that in the long run we might
wish what is logically representable as RSS to be portable
from. The question of whether to use XML signature remains worth
discussing and investigating.)

