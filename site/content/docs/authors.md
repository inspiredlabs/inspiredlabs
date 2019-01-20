---
date: 2017-09-26T06:00:00+06:00
lastmod: 2017-10-11T17:30:00+06:00
title: Authors Setup Guide
authors: ["muniftanjim"]
categories:
  - features
tags:
  - authors
slug: authors
---

# 3si
## Stoke-on-trent, 2015
### Who are 3Si, and what they do?

Derived from their surname Chris Sinclair, Pete Sinclair, and their Father – a silent partner, [3Si](https://inspiredlabs.co.uk/3-si.com/) sell their CRM application called OM.Net for handling large volumes of membership and subscription data.

### Legacy of the project

A static site template with a fresh perspective on their marketing material, whilst honouring what is already in use.

> Scott fully understands the concepts of design…
    how things flow and the way the message is conveyed to the user.
    – Chris Sinclair Managing Director, 3Si 
    
Explore

[Marketing Brochure](https://inspiredlabs.co.uk/3-si.com/print/3si-infosheets-draft.pdf)

Visit

[3Si.com](https://inspiredlabs.co.uk/3-si.com/) [Marketing Brochure](https://inspiredlabs.co.uk/3-si.com/print/3si-infosheets-draft.pdf)

Minimo supports multiple authors for your site. Just make sure you have the following configuration in your site's **`config.toml`**:

```toml
[taxonomies]
author = "authors"
```

Minimo treats Authors as a [Hugo Taxonomy](https://gohugo.io/content-management/taxonomies/).

## Author's Profile

For adding an author to your site:

- Create **`data/authors`** folder in your site's root directory
- Create a file with the filename format: **`<username>.toml`**

Now, add information about the author using the structure below:

**/data/authors/muniftanjim.toml**

{{< file "data/authors/muniftanjim.toml" >}}

_You can use either the `[email]` fields or the `[social.email]` field. You don't need to fill them both. However, it is encouraged to use `[email]` instead of `[social.email]`._

## Adding Authors to Contents

For adding authors to your content include the following option in your content's front-matter:

```yaml
---
authors: ["muniftanjim"]
---
```

- `authors` [`Array` of `String`s]: username of authors

That's all.
