---
layout: post
title: "Code reuse across projects"
tags: [programming]
---
{% include JB/setup %}

At GA we need to reuse little snippets of code. It's not projects, it's not subparts of a gem, they are small snippets. Constants, email normalization and validation, network errors handler, shared cookies and associated custom behavior, background job exceptions notifiers, deploy scripts, and the like. Not complex enough to abstract completely, nor simple enough to go ahead and write it.

Each snippet no more than 50 lines of code, at most just a simple value string –but apps' stability depend on it. Until now we copy them where needed. Many bits are entangled together across project, with their own release cycles, their own flows and styles, their own priorities, their own teams for short. Discovered a better way to handle network errors? Good luck finding out if each project is using it! The dreads of duplication.

It's not worth it to package each script separately and make apps depend on all, not cool to bundle them up in well defined bigger packages which serve their own well-defined purpose, not nice to define a `GA::JUNK_DRAWER` gem. Junk drawers are messy, can be as useful as can be garbage you throw out for unused.

Naming bites, while discussing my team mate took it seriously to my surprise: "that's not the best name, can be the top level `GA`". After all, a gem doesn't need to include all it's files, parts may be used wherever needed by just including it's parts, much like rails or any of it's frameworks. After all, the `Rails` wrapper is the one that makes _all that code_ work together smoothly. See for example [how to use parts of `ActiveSupport`](http://guides.rubyonrails.org/active_support_core_extensions.html).

Now we can have a gem with controllers error handling, models validation, authentication configurations, cookies handling, popular gems extensions which didn't make it to master, etc. Each as a separate concern, all in one gem.
