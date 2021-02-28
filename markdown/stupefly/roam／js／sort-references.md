- {{{[[roam/js]]}}}
    - ```javascript

var existing = document.getElementById("sort-references");
if (!existing) {
  var extension = document.createElement("script");
  extension.src = "https://roamjs.com/sort-references.js";
  extension.id = "sort-references";
  extension.async = true;
  extension.type = "text/javascript";
  document.getElementsByTagName("head")[0].appendChild(extension);
}
```
- Default Sort:: Page Title
