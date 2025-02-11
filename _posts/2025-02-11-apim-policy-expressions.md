---
title: "Azure APIM Policy Expressions"
date: 2025-02-11
layout: post
---

# Common Expressions
## Http Headers
| Description | Snippet |
| ----------- | ----------- |
| Get a HTTP Header | `context.Request.Headers.GetValueOrDefault("header-name","optional-default-value")` |
| Check Header Existence | `context.Request.Headers.ContainsKey("header-name") == true` |
| Check if header has expected value | `context.Request.Headers.GetValueOrDefault("header-name", "").Equals("expected-header-value", StringComparison.OrdinalIgnoreCase)` |
