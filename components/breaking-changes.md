---
collection: docs
title: Breaking Changes
order: 2
---

### 20-04-2015: userFields introduced in Auth config (RG-640) 

It's now required to set userFields Auth's config if fields other than `id,name,profile` are needed in auth.requestUser.

Example:
```js
var auth = new Auth({
  serverUri: 'http://localhost/',
  userFields: ['avatar', 'profile']
});
```