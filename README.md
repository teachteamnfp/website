[![Deploy to Azure](http://azuredeploy.net/deploybutton.png)](https://azuredeploy.net/)





The New elementary.io
================

[![Bountysource](https://www.bountysource.com/badge/tracker?tracker_id=10548672)](https://www.bountysource.com/trackers/10548672-elementary-website)
[![Build Status](https://travis-ci.org/elementary/website.svg?branch=master)](https://travis-ci.org/elementary/website)
[![Translation status](https://l10n.elementary.io/widgets/website/-/svg-badge.svg)](https://l10n.elementary.io/engage/website/?utm_source=widget)

A focused, minimum viable product (hence MVP) for a website that accompanied the release of elementary OS Freya.

Project Organization
====================

* **Issues** for individual actionable items, or bugs i.e.:
  * Design home page
  * Implement home page
  * Add payment form
  * Fix link to Wired article
* **Milestones** for "releases" or overall steps, i.e.:
  * Single-page site
  * User Documentation
  * Journal
* **Reviews** Do all work in branches, then submit pull requests for review when ready
  * No dummy content in master, ever.
  * small diff is best diff
  * The reviewer is the gatekeeper. Be kind of a dick.


Architecture/Philosophies
=========================

* HTML, CSS, and JS
* Super simple PHP-based templating system
* No/minimal frameworks (keep it simple!)
* Graceful degradation (don't be held back by crappy browsers)
* Mobile-first


Templating System
=================

* PHP-based
* Pages go in root as .php files
* `require_once '_backend/preload.php';`, set any variables, then `include $template['header'];` (see [code-of-conduct](https://github.com/elementary/website/blob/master/code-of-conduct.php) for an example) at top of page.
* `include $template['footer'];` at bottom of page.
* Page variables:
  * `$page['title']`
  * `$page['description']`
  * `$page['author']`

Contributing
============

See guidelines for [coding](https://github.com/elementary/website/blob/master/.github/CONTRIBUTING.md) and [translating](https://github.com/elementary/website/blob/master/TRANSLATE.md).

Security
========

For any security related issues, please **do not open a public GitHub issue**. Instead, email them to [webmaster@elementary.io](mailto:webmaster@elementary.io). We will provide an initial assessment of security reports within 48 hours and should apply patches within 2 weeks (also, feel free to contribute a fix for the issue).

License
=======

This project has a [MIT license](LICENSE.md).
