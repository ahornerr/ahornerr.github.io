---
layout: default
---

I’m a developer who builds software and automation to solve practical problems. Here are a few of my projects and open source contributions.

## Open Source Projects

### [CutScene](https://github.com/ahornerr/CutScene)
I built CutScene because sharing a moment from Plex meant opening the file in VLC, hunting for the timestamp, and converting the clip to MP4. Now I preview, trim, and export clips in the browser, and I use it regularly.

I also built a [semantic search prototype](https://github.com/ahornerr/CutScene/pull/17) for when I remember the gist of a line but not the exact words. It indexes timestamped subtitles in PostgreSQL with pgvector, combines exact matches with semantic results, and points back to the moment in Plex.

### [TileWhisper](https://github.com/ahornerr/TileWhisper)
I built a RuneLite plugin that lets nearby players talk in Old School RuneScape. The project went beyond the plugin: I set up the [voice relay](https://github.com/ahornerr/TileWhisperServer), hosting, domain, and analytics.

### [Krogetter](https://github.com/ahornerr/krogetter)
I wanted to know when Vanilla Coke Zero went on sale. That turned into a tool that tracks offers at Kroger-family stores and surfaces them in Home Assistant.

Earlier work: [go-dash-button](https://github.com/ahornerr/go-dash-button), a library and sample application for triggering events when Amazon Dash buttons connect to WiFi.

{% assign psize = site.posts | size %}
{% if psize > 0 %}
## Project Blog Posts

{% for post in site.posts %}
### [{{post.title}}]({{post.url}})
{{post.excerpt}}
{% endfor %}
{% endif %}

## Selected Open Source Contributions

* [gorilla/handlers: Remove the Content-Encoding response header when responding with a HTTP 204 or 304](https://github.com/gorilla/handlers/pull/176)
* [emersion/go-imap: Add support for raw search fields](https://github.com/emersion/go-imap/pull/334)
* [sgreben/slack-emoji-upload: Use Slack API provided rate limit Retry-After value](https://github.com/sgreben/slack-emoji-upload/pull/1)

[Browse the full contributions archive]({{ '/contributions.html' | relative_url }}).
