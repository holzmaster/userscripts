---
layout: post
title: "ProTagFilter"
categories:
  - userscript
author: ioPr0Skill
presented: 2282883
link: //github.com/pr0Skill/ProTagFilter/blob/master/ProTagFilter.js
code: //github.com/pr0Skill/ProTagFilter
---

Es Ermöglicht das automatische überspringen bzw downvoten anhand bestimmter Tags und ihrer jeweiligen Gewichtung.

```javascript
var ignoreTags = [{
  tag: 'repost', // wer mag schon reposts?
  downvote: true, // automatisch runter Voten?
  skip: false, // überspringen
  confidenceThreshold: 0.85 // ab welcher confidence ( > mehr upvots < weniger )
}];
```