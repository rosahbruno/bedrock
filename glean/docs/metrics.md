<!-- AUTOGENERATED BY glean_parser. DO NOT EDIT. -->

# Metrics

This document enumerates the metrics collected by this project using the [Glean SDK](https://mozilla.github.io/glean/book/index.html).
This project may depend on other projects which also collect metrics.
This means you might have to go searching through the dependency tree to get a full picture of everything collected by this project.

# Pings

- [interaction](#interaction)
- [non-interaction](#non-interaction)
- [page-view](#page-view)

## interaction

A ping which is sent when a page element is
interacted with.


This ping includes the [client id](https://mozilla.github.io/glean/book/user/pings/index.html#the-client_info-section).

**Data reviews for this ping:**

- <https://bugzilla.mozilla.org/show_bug.cgi?id=1767442>

**Bugs related to this ping:**

- <https://github.com/mozilla/bedrock/issues/10746>

All Glean pings contain built-in metrics in the [`ping_info`](https://mozilla.github.io/glean/book/user/pings/index.html#the-ping_info-section) and [`client_info`](https://mozilla.github.io/glean/book/user/pings/index.html#the-client_info-section) sections.

In addition to those built-in metrics, the following metrics are added to the ping:

| Name | Type | Description | Data reviews | Extras | Expiration | [Data Sensitivity](https://wiki.mozilla.org/Firefox/Data_Collection) |
| --- | --- | --- | --- | --- | --- | --- |
| element.clicked |[event](https://mozilla.github.io/glean/book/user/metrics/event.html) |An event containing metrics related to which element in the page was clicked.  |[Bug 1767442](https://bugzilla.mozilla.org/show_bug.cgi?id=1767442)|<ul><li>label: Description of the page element that was clicked. Examples: 'Download Firefox', 'Get Mozilla VPN'. </li><li>position: The position of the element in the page. Examples: 'Primary', 'Secondary', 'Navigation', 'Footer'. </li><li>type: The type of element that was clicked. Examples: 'Button', 'Link'. </li></ul>|never |3 |
| page.locale |[string](https://mozilla.github.io/glean/book/user/metrics/string.html) |The locale of the page that was viewed.  |[Bug 1767442](https://bugzilla.mozilla.org/show_bug.cgi?id=1767442)||never |3 |
| page.page_event |[event](https://mozilla.github.io/glean/book/user/metrics/event.html) |An event containing metrics related to a page level completion or state that want to measure. This can be sent in either an interaction and non-interaction ping, depending upon the use-case. Examples: form completion, scroll events, banner impressions.  |[Bug 1767442](https://bugzilla.mozilla.org/show_bug.cgi?id=1767442)|<ul><li>label: The label used to describe the event. Example: 'Newsletters: mozilla-and-you' </li><li>type: The type of event. Example: 'Newsletter Signup Success' </li></ul>|never |3 |
| page.path |[string](https://mozilla.github.io/glean/book/user/metrics/string.html) |The URL path of the page that was viewed, excluding locale.  |[Bug 1767442](https://bugzilla.mozilla.org/show_bug.cgi?id=1767442)||never |3 |
| page.query_params |[labeled_string](https://mozilla.github.io/glean/book/user/metrics/labeled_strings.html) |Query parameters associated with the URL of the page that was viewed.  |[Bug 1767442](https://bugzilla.mozilla.org/show_bug.cgi?id=1767442)|<ul><li>utm_source</li><li>utm_campaign</li><li>utm_medium</li><li>utm_content</li><li>entrypoint_experiment</li><li>entrypoing_variation</li><li>experiment</li><li>variation</li><li>v</li><li>xv</li></ul>|never | |
| page.referrer |[string](https://mozilla.github.io/glean/book/user/metrics/string.html) |The referring URL that linked to the page that was viewed.  |[Bug 1767442](https://bugzilla.mozilla.org/show_bug.cgi?id=1767442)||never |3 |
| page.viewed |[datetime](https://mozilla.github.io/glean/book/user/metrics/datetime.html) |The time a page was viewed.  |[Bug 1767442](https://bugzilla.mozilla.org/show_bug.cgi?id=1767442)||never |3 |

## non-interaction

A ping which is sent when a non-user initiated event
occurs. Examples: a specific banner impression is
displayed, a video auto-plays on scroll.


This ping includes the [client id](https://mozilla.github.io/glean/book/user/pings/index.html#the-client_info-section).

**Data reviews for this ping:**

- <https://bugzilla.mozilla.org/show_bug.cgi?id=1767442>

**Bugs related to this ping:**

- <https://github.com/mozilla/bedrock/issues/10746>

All Glean pings contain built-in metrics in the [`ping_info`](https://mozilla.github.io/glean/book/user/pings/index.html#the-ping_info-section) and [`client_info`](https://mozilla.github.io/glean/book/user/pings/index.html#the-client_info-section) sections.

In addition to those built-in metrics, the following metrics are added to the ping:

| Name | Type | Description | Data reviews | Extras | Expiration | [Data Sensitivity](https://wiki.mozilla.org/Firefox/Data_Collection) |
| --- | --- | --- | --- | --- | --- | --- |
| page.locale |[string](https://mozilla.github.io/glean/book/user/metrics/string.html) |The locale of the page that was viewed.  |[Bug 1767442](https://bugzilla.mozilla.org/show_bug.cgi?id=1767442)||never |3 |
| page.page_event |[event](https://mozilla.github.io/glean/book/user/metrics/event.html) |An event containing metrics related to a page level completion or state that want to measure. This can be sent in either an interaction and non-interaction ping, depending upon the use-case. Examples: form completion, scroll events, banner impressions.  |[Bug 1767442](https://bugzilla.mozilla.org/show_bug.cgi?id=1767442)|<ul><li>label: The label used to describe the event. Example: 'Newsletters: mozilla-and-you' </li><li>type: The type of event. Example: 'Newsletter Signup Success' </li></ul>|never |3 |
| page.path |[string](https://mozilla.github.io/glean/book/user/metrics/string.html) |The URL path of the page that was viewed, excluding locale.  |[Bug 1767442](https://bugzilla.mozilla.org/show_bug.cgi?id=1767442)||never |3 |
| page.query_params |[labeled_string](https://mozilla.github.io/glean/book/user/metrics/labeled_strings.html) |Query parameters associated with the URL of the page that was viewed.  |[Bug 1767442](https://bugzilla.mozilla.org/show_bug.cgi?id=1767442)|<ul><li>utm_source</li><li>utm_campaign</li><li>utm_medium</li><li>utm_content</li><li>entrypoint_experiment</li><li>entrypoing_variation</li><li>experiment</li><li>variation</li><li>v</li><li>xv</li></ul>|never | |
| page.referrer |[string](https://mozilla.github.io/glean/book/user/metrics/string.html) |The referring URL that linked to the page that was viewed.  |[Bug 1767442](https://bugzilla.mozilla.org/show_bug.cgi?id=1767442)||never |3 |
| page.viewed |[datetime](https://mozilla.github.io/glean/book/user/metrics/datetime.html) |The time a page was viewed.  |[Bug 1767442](https://bugzilla.mozilla.org/show_bug.cgi?id=1767442)||never |3 |

## page-view

A ping which is sent everytime a page is viewed.


This ping includes the [client id](https://mozilla.github.io/glean/book/user/pings/index.html#the-client_info-section).

**Data reviews for this ping:**

- <https://bugzilla.mozilla.org/show_bug.cgi?id=1767442>

**Bugs related to this ping:**

- <https://github.com/mozilla/bedrock/issues/10746>

All Glean pings contain built-in metrics in the [`ping_info`](https://mozilla.github.io/glean/book/user/pings/index.html#the-ping_info-section) and [`client_info`](https://mozilla.github.io/glean/book/user/pings/index.html#the-client_info-section) sections.

In addition to those built-in metrics, the following metrics are added to the ping:

| Name | Type | Description | Data reviews | Extras | Expiration | [Data Sensitivity](https://wiki.mozilla.org/Firefox/Data_Collection) |
| --- | --- | --- | --- | --- | --- | --- |
| page.locale |[string](https://mozilla.github.io/glean/book/user/metrics/string.html) |The locale of the page that was viewed.  |[Bug 1767442](https://bugzilla.mozilla.org/show_bug.cgi?id=1767442)||never |3 |
| page.path |[string](https://mozilla.github.io/glean/book/user/metrics/string.html) |The URL path of the page that was viewed, excluding locale.  |[Bug 1767442](https://bugzilla.mozilla.org/show_bug.cgi?id=1767442)||never |3 |
| page.query_params |[labeled_string](https://mozilla.github.io/glean/book/user/metrics/labeled_strings.html) |Query parameters associated with the URL of the page that was viewed.  |[Bug 1767442](https://bugzilla.mozilla.org/show_bug.cgi?id=1767442)|<ul><li>utm_source</li><li>utm_campaign</li><li>utm_medium</li><li>utm_content</li><li>entrypoint_experiment</li><li>entrypoing_variation</li><li>experiment</li><li>variation</li><li>v</li><li>xv</li></ul>|never | |
| page.referrer |[string](https://mozilla.github.io/glean/book/user/metrics/string.html) |The referring URL that linked to the page that was viewed.  |[Bug 1767442](https://bugzilla.mozilla.org/show_bug.cgi?id=1767442)||never |3 |
| page.viewed |[datetime](https://mozilla.github.io/glean/book/user/metrics/datetime.html) |The time a page was viewed.  |[Bug 1767442](https://bugzilla.mozilla.org/show_bug.cgi?id=1767442)||never |3 |

Data categories are [defined here](https://wiki.mozilla.org/Firefox/Data_Collection).

<!-- AUTOGENERATED BY glean_parser. DO NOT EDIT. -->
