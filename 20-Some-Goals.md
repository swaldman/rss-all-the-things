# Some Goals

- RSS applications should be capable of constituting elements of a
  blogosphere, a microblogosphere,
  [artcasting](http://scripting.com/2023/11/17.html),
  [textcasting](https://textcasting.org/), product review systems
  (e.g. Yelp, TripAdvisor, etc.), and more. RSS items should permit
  annotation with the application-specific metadata these applications
  require in a standard way. Advanced RSS clients or third-party
  aggregators could index these items to provide
  application-appropriate search and discovery. Although third-party
  aggregators constitute a potential locus of enclosure and
  centralization, author-owned content items with standard annotations
  mean no platform can *exclusively* index and serve the content.
- Dynamic applications should be able to generate and modify feeds and
  respond on behalf of multiple HTTP virtual hosts. Each feed should
  generates links consistent with the owning host, rather than the hostname of the service. 
  A clients modifying
  state identifies itself with a DNS hostname. If the client’s
  identity is hosted by the application, the application should
  generate feeds reflecting in links the client’s
  ownership. If the client’s identity is hosted elsewhere,
  applications should update its own state, but update
  the owning identity’s hosting service, if one is provided.
  In this way, items like blog comments can be kept in sync across
  multiple relevant services.
