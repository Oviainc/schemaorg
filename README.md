# Ovia Inc — Schema.org (fork of schemaorg/schemaorg)

![Ovia Inc — Schema.org icon from the upstream project assets](docs/schemaicon.png)

We maintain this fork of [schemaorg/schemaorg](https://github.com/schemaorg/schemaorg), the project repository behind Schema.org: all of the schemas, examples, and software used to publish the Schema.org vocabulary. The vocabulary gives the web a shared, machine-readable way to describe things — organisations, products, services, events, places, creative work, and much more — in formats such as JSON-LD, Microdata, and RDFa, so that search engines and other data consumers can read a page as structured data rather than as text alone. Upstream credit: the Schema.org project, its steering group, and the W3C Schema.org Community Group and contributors. Licence: Apache-2.0 (see LICENSE).

**Our main site:** https://oviainc.github.io/ai-services/

**Upstream repository:** https://github.com/schemaorg/schemaorg

## What this is

The vocabulary source itself, held as working files rather than as a finished website:

- `data/schema.ttl`, the main schemas file, written in W3C RDFS in RDF/Turtle format, with per-topic example files beside it (`data/*examples.txt`) covering areas from hotels, books, and courses to invoices, datasets, menus, and video games.
- `data/releases/` and `versions.json`, the release record: the fork snapshot carries schema version 29.4, released December 8, 2025, at the top of a release log that runs back to version 7.0 in 2020.
- `software/`, the publishing software (Python, with the supporting application imported as the `sdopythonapp` submodule) that builds a static copy of the Schema.org site for review and release, plus `docs/` and `templates/` for the published documentation.
- Supporting vocabulary files such as `data/mappings.ttl` and `data/extdefs.jsonld`, which record how Schema.org terms align with external vocabularies.

The published vocabulary lives at https://schema.org/ — the homepage already recorded on this fork, verified live at this pass. Upstream carries about 6,316 stars and 975 forks at the time of this pass, and the project makes a formal release every month or so after review by the Schema.org Steering Group and the wider community, per the upstream notes preserved below.

## Story

Schema.org launched in 2011 as a shared vocabulary project, and the upstream GitHub repository opened on January 30, 2014, as the place where every change to the site is discussed and made. The upstream README preserved below records the working style that shaped the vocabulary: simple, backwards-compatible improvements to existing terms are favoured over new vocabulary, new terms need evidence that a consuming application will use the data, and local coherence — a sensible way to describe a common situation — wins over global elegance. Terms often arrive in a Pending area first, gather feedback, and then settle into the core vocabulary through the release process.

We forked the project on January 18, 2026, at the January 16, 2026 snapshot (tip commit e5f59b2, an example and documentation update for member tiers), into the knowledge and research group of the Oviainc collection. In role, this fork is the structured-data shelf of that group: where the general reference shelf maps tools and the company-landscape shelf maps companies, this fork holds the vocabulary that describes both — the shared terms a site, a dataset, or an agent uses to say what a thing is in a form machines can act on.

What we evaluate here is the vocabulary as a working input, with its limits kept visible:

- **Coverage for business descriptions** — how completely the core and Pending terms describe the things our sites and client-facing pages need to state: an organisation, its services and offers, locations, events, frequently asked questions, and articles, and where the vocabulary still leaves gaps.
- **Examples as the practical layer** — the per-topic example files show each term in JSON-LD, Microdata, and RDFa in real page situations; the examples, more than the term definitions alone, show what correct structured data looks like when published.
- **Release discipline as a pattern** — a dated release log, release snapshots held in the repository, staging previews, and a monthly-or-so cadence governed by a steering group: a long-running example of a shared vocabulary changing without breaking the pages that already use it.
- **Alignment files** — `mappings.ttl` and the extension definitions show how one vocabulary maps onto others, the same alignment problem that appears whenever two datasets or two agent tools describe the same thing with different terms.

Where the project fits our work:

- **AI agents** — agents act on structured descriptions of the world; a shared vocabulary for organisations, products, actions, and events is part of how agent-readable pages and tool outputs stay unambiguous.
- **Context engineering** — structured data is context in its most disciplined form: typed terms with defined meanings, held in files that both people and machines can check, rather than meaning carried by prose alone.
- **Business intelligence and data** — the vocabulary underpins knowledge-graph and dataset work, and the term and mapping files are a reference when a dataset needs a public, stable set of types and properties instead of a private one.
- **Virtual production** — a lighter fit: the vocabulary carries media and creative-work terms (video, broadcast, music, and screening events all appear in the examples), and the shelf is a first check when a production page or catalogue needs structured descriptions.

The direct line to our own work is search: the ai-services site and the wider site family rely on structured data so that search engines read each page correctly, and this fork is the reference shelf that work checks against — the plan for this pass records the fork exactly that way, as relevant to the SEO work on ai-services and otherwise a reference.

## Modifications by Ovia Inc

Documentation only. Upstream schemas, examples, and software are unchanged from the fork point, except for documentation notes added in November 2026: a modification reference on November 4, 2026, replaced by this expanded treatment (Ovia section, story, picture, and repository details) on November 22, 2026. Where a later commit in this repository says otherwise, that commit governs.

## Sync status

Behind upstream, by design of this pass. This fork carries the January 16, 2026 snapshot (tip commit e5f59b2) plus documentation commits of our own (November 4, 2026, replaced and expanded November 22, 2026), for 5,641 commits in total at the November 4, 2026 documentation commit. Upstream stands at 5,741 commits with HEAD ba90187 (November 20, 2026), so the fork stands ahead by the documentation commits only and behind by 101 commits. The upstream distance is ordinary vocabulary and software work across ten months of releases and fixes, so a sync here is a snapshot adoption rather than a small merge; no sync was applied in this pass, and a reviewed sync is recommended for Ja when the reference shelf needs the current vocabulary.

## Related repositories

- [ai-services](https://github.com/Oviainc/ai-services) — our flagship site: AI agents, machine learning in production, and AI products for business; the structured-data and SEO work there is the main consumer of this shelf
- [artificial-intelligence](https://github.com/Oviainc/artificial-intelligence) — our learning and reference hub, with guides across agents, context engineering, data, and virtual production
- [Ovias-Fork-The-book-of-secret-knowledge](https://github.com/Oviainc/Ovias-Fork-The-book-of-secret-knowledge) — the general reference shelf of the knowledge and research group: a curated collection of lists, manuals, cheatsheets, and tools for operators
- [oviainc-open-source-companies](https://github.com/Oviainc/oviainc-open-source-companies) — the company-landscape shelf of the knowledge and research group: a generated list of open source startups funded by Y Combinator
- [Agent-Reach-ovia-inc](https://github.com/Oviainc/Agent-Reach-ovia-inc) — the outward read layer of the knowledge and research shelf: internet reach across social platforms, search, and code hosts without API fees

## Working with us

Start from our site: https://oviainc.github.io/ai-services/ — the contact form there is the fastest way to reach us.

## Licence

Apache-2.0, as recorded in the LICENSE file in this fork and upstream. Upstream credit remains with the Schema.org project and contributors; regarding Creative Commons and open-source licensing for documents and software, upstream points to the FAQ entry preserved in the README below.

---

Ovia Inc — Artificial Intelligence & Context Engineering. Based in Canada, working wherever the work is.

---

Welcome to Schema.org
=====================
[![CI Tests Shield](https://github.com/schemaorg/schemaorg/actions/workflows/ci_tests.yml/badge.svg)](https://github.com/schemaorg/schemaorg/actions)


# Important Links and Official Channels
- [The Schema.org Website (https://schema.org/)](https://schema.org/)
- [The Schema.org Blog (https://blog.schema.org/)](https://blog.schema.org/)
- [Releases and Release History (https://schema.org/docs/releases.html)](https://schema.org/docs/releases.html)

# Introduction
This is the Schema.org project repository. It contains all the schemas, examples and software used to publish Schema.org. For the site itself, please see [Schema.org](https://schema.org/) instead.

Note: Much of the supporting software is imported from a sub-module: 'sdopythonapp'

Issues and proposals are managed here by collaborators around the project, especially participants of the [W3C Schema.org Community Group](https://www.w3.org/community/schemaorg/). If you are interested in participating please
join the group at the [W3C](https://www.w3.org/community/schemaorg/), introduce yourself and find or file issues here that engage your interest. If you are new to Git and Github, there's a useful [introduction to Github](https://www.w3.org/2006/tools/wiki/Github) in the W3C Wiki.

There are also continuous integration tests to check incoming pull requests.

[Issue #1](https://github.com/schemaorg/schemaorg/issues/1) in Github is an entry point for release planning. It
should provide an overview of upcoming work in terms of broad themes, specific issues and release milestones.

[Issue #1](https://github.com/schemaorg/schemaorg/issues/1) will link to per-release entry points, or else navigate issues via label or milestone within Github.
Every change to the site comes via discussions here. Substantive changes are recorded in our [release notes](https://schema.org/docs/releases.html).
A preview of the [draft new release notes](https://staging.Schema.org/docs/releases.html) can be found as part of the test site for our next release.
Every month or so, after final review by the Schema.org Steering Group and wider community, we make a formal release.

Regarding CC and opensource licenses for documents and software, see our [FAQ entry](https://schema.org/docs/faq.html#18).

We have a [blog](https://blog.Schema.org/) for communication of interesting updates to Schema.org.

Improving schemas
=================

We are always interested in practical suggestions for improvements to Schema.org, and our collection of schemas has been [growing gradually](http://schema.org/docs/releases.html) since our launch in 2011.

We try to [prioritize](https://lists.w3.org/Archives/Public/public-schemaorg/2015Dec/0016.html) simple fixes and improvements to our existing schemas, examples and documentation over the addition of new vocabulary, and we are most likely to add new schemas when there is evidence that some (preferably large-scale) consuming application will make use of the data. Consuming applications need not be search engines; software tools e.g. opensource, markup-enriched approaches to web analytics, browser add-ons or cloud tools are all rich areas for exploration and collaboration. The important thing is that there should be some reasonable expectation of data consumers making good use of the changes. It is not sufficient to justify additions on the basis that search engines generally try to use Schema.org-based structured data. Smaller changes, and backwards-compatible changes, are easier to incorporate.

Note that Schema.org does *not* attempt to capture the full detail of ceb content; it is necessarily a simplification of a more complex reality. This means that there will be many cases where adding more detail to Schema.org will look possible. However, in the interests of keeping Schema.org simple and usable for publishers and webmasters, we will often choose not to add such detail. Schema.org uses web standards such as JSON-LD, Microdata and RDFa to
allow for [independent extension](http://schema.org/docs/extension.html) (for example, see [GS1's vocabulary](https://ref.gs1.org/voc/)).

We are also highly unlikely to take on large-scale reorganizations of Schema.org's terminology if they are motivated solely by considerations of elegance, "proper modeling", ontological purity or conceptual unification. Although the project founders and team are familiar with - and respectful of - the traditions behind such concerns, the scale, scope and nature of Schema.org have required us to trade elegance and global consistency for a somewhat scruffier notion of incremental evolution and a pragmatic tolerance for a style that would be out of place in a formal ontology. Proposals for unifying cross-domain logic-based knowledge structures may be better received (e.g. in the [Ontolog](https://groups.google.com/g/ontolog-forum) community).

We sometimes introduce types without dedicated property associations, simply for markup usability reasons. In a formal ontology, this is often considered poor modeling. However, logically equivalent structures can result in many more errors from publishers/webmasters unfamiliar with the underlying formal concepts behind JSON-LD or RDF/S. Schema.org is not a closed system, and other initiatives e.g. Wikidata or [GS1](https://ref.gs1.org/voc/) have defined many other terms that can be mixed in alongside those we define at Schema.org. We also make efforts to align our designs to relevant external standards and initiatives, even when it reduces the global elegance of Schema.org considered alone. For example in a bibliographic or cultural heritage context, we may be influenced by initiatives like MARC, BibFrame, and FRBR, while for e-commerce, we collaborated with [Good Relations](https://blog-Schema.org/2012/11/08/good-relations-and-schema-org/) and GS1. Schema.org's [news](https://schema.org/docs/news.html)-related terms were heavily influenced by incorporating [IPTC's rNews](https://iptc.org/standards/rnews/) design, alongside collaborations with [fact checkers](https://www.poynter.org/product-category/fact-checking/), the [Trust Project](https://thetrustproject.org/), and others. Our TV and Music related vocabularies are heavily influenced by working with the [BBC and the European Broadcasting Union](https://www.bbc.co.uk/ontologies), alongside [the Music ontology](http://musicontology.com/docs/getting-started.html) and [MusicBrainz](https://musicbrainz.org/doc/LinkedBrainz/RDF); our schemas reflect these prior designs. We prefer to collaborate in this way, improving Schema.org incrementally and working to polish, integrate and blend such designs rather than produce our own pure model in isolation. The result may lack global elegance but brings our work into alignment with related efforts worldwide.

We always welcome issues that track usability and readability issues, but encourage a focus on concrete situations (e.g. how to describe repeating events) rather than global philosophical concerns (e.g. whether a `Reservation` or `Action` is "really" an `Event`). We prioritize local coherence (having sensible ways to describe many common situations) over global elegance (having a global theory in which everything has a sensible place). This doesn't mean we never have cleanups, but they are balanced against (and often outweighed by) other considerations.

When we add terms, often into the "Pending" area, we strongly encourage feedback that takes a global perspective: how does a new term relate to others, how could it be used alongside pre-existing patterns, etc. The changes we make during this integration phase reflect such considerations, but are usually expressed through modest rewording, examples, or adjustments to the documentation of type/property links, rather than through major restructuring.

 * Suggestions for improvements are always welcome here - please search for older discussions (including closed issues) before opening a new issue.
 * We particularly value improvements to existing definitions, examples and text, to clarify how Schema.org vocabulary is used in practice.
 * Please don't be surprised or offended if you raise an issue proposing new schemas and it is marked by the project team as "[noted](https://github.com/schemaorg/schemaorg/issues?q=is%3Aissue+label%3A%22Closed+and+Noted+%28and+possibly+Queued%29%22+is%3Aclosed)" then closed. We have 100s of issues discussing possible improvements, and to keep things manageable we adopt the convention of noting then closing issues that are not likely to be immediately explored.
 * While many Schema.org improvements have been proposed via Github's "[Pull request](https://help.github.com/articles/about-pull-requests/)" mechanism (see also our list of [PRs](https://github.com/schemaorg/schemaorg/pulls)), please do not undertake any substantial development work without agreeing it with the project team here first.
 * All Pull Requests should reference specific issues that they're fixes or solutions for. This lets the Schema.org community discuss problems and topics without it being tied too closely to a specific (and easily outdated) proposed fix.
 * Please note that some changes are much easier to make than others: the wording/phrasing in definitions is relatively easy to amend, whereas the exact spelling of a type or property ('Person', 'startDate' etc.) is much more disruptive to change.
 * There are many other projects developing schemas and ontologies for the Web, e.g. [Wikidata](http://wikidata.org/) or the vocabulary projects in the [Linked Data](https://lov.linkeddata.es/dataset/lov/) community. Many of these projects go into more expressive detail than is possible for a project like Schema.org. To keep Schema.org manageable, we have a strong bias towards designs that are grounded in large scale usage on the Web, in particular [usage](https://github.com/schemaorg/schemaorg/issues/652) by data-consuming applications since these in turn motivate data publishers. Other schema initiatives have different priorities and make different tradeoffs.

See more on ["How we work"](https://schema.org/docs/howwework.html)


Software
========

For most collaborators, all you need to know about the software is how to run it. 

The objective of the software is to create a static copy of the Schema.org site, including potential local changes, to inspect and run behind a simple web server on a local system for testing.  In the same way that a production release is deployed to a cloud server, your local version could then be deployed to a virtual machine using gcloud to enable collaboration with others.

Full instructions are available in [SOFTWARE_README.md](software/SOFTWARE_README.md) explaining how to create the initial local copy to work with, then evolve to test out any changes.

Essentially you will need to have a Linux-like (inc  Mac) environment loaded with Python version 3.6 or above. You can then make test builds of Schema.org running on your own machine accessible as http://localhost:8080/ or else post them on appspot.com for collaboration. See the [Appengine documentation](https://cloud.google.com/appengine/docs) for details of the relevant gcloud commands.

More detailed information about the software is available in [SOFTWARE_README.md](software/SOFTWARE_README.md).

See also notes in the wiki: https://github.com/schemaorg/schemaorg/wiki/Contributing

Formats and standards
=====================

All schemas and examples are in data/ in utf-8 encoded files.

The main schemas file is data/schema.ttl (utf-8)

While developing schemas, using data/sdo-somethinghere-schema.ttl can be useful.

The format is based on W3C RDFS in RDF/Turtle format.

The examples are stored in data/examples.txt (utf-8) and other *.txt files.

As with schemas, data/*examples.txt will also be read. It can be useful to develop
using separate files. When vocabulary is finally integrated into the main repository, schema
data will be merged into Schema.org. However, examples will stay in separate files, as this
works better with git's file comparison machinery.

The data/releases/ hierarchy is reserved for release snapshots (see https://schema.org/version/).

The ext/*/ hierarchy is reserved for extensions (see https://schema.org/docs/extension.html).


We no longer use Github branches for work-in-progress. The main/ branch is our latest candidate. It is not guaranteed to be in a conceptually consistent state, but should stabilize prior to circulation of a release candidate for review.

Notes
=====

This documentation concerns the software codebase rather than Schema.org itself.

However, do note that labels, comments, and documentation should use US English (in the code
and schemas). If a choice between English variants is needed, aim for international
English wherever possible.

