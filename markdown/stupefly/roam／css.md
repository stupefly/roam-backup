- ```css
/*  Make sure you have the fonts Lato, Open Sans, and IBM Plex installed locally on your machine.
They're free to download from Google:
https://fonts.google.com/specimen/Lato
https://fonts.google.com/specimen/Open+Sans
https://fonts.google.com/featured/Plex
*/


 :root {
    --header-font:"Lato", sans-serif;
    --body-font:"Open Sans", sans-serif;
    --code-font:"IBM Plex", monospace;
    --font-size: 0.95rem;
    --bg-color: #F8F9FB;
    --page-color: rgba(255, 255, 255, 0.95);
    --text-color: #3f4758;
    --light-text-color: #7086A9;
    --page-tag-color: #9DAFCA;
    --color-primary: #ec6f35;
    --color-primary-light: #ff913c;
    --color-primary-highlight: #fcc1786d;
    --color-secondary: #7056F2;
    --color-subtle-border: #dbe4e8;
}

/* Body Colours */
body, #app {
  background: var(--bg-color);
}
.roam-article {
  padding-right: 10px !important;
  max-width: 740px;
  padding-left: 20px !important;
}
.roam-article > div {
  padding: 30px 50px 50px 50px;
  background: var(--page-color);
  box-shadow: var(--page-shadow);
  border: 1px solid #e5ecf1;
  border-radius: 6px;
  margin-top: 10px !important;
  width: auto;
}
.roam-body-main {
  top: 0 !important;
  height: 100% !important;
  width: auto !important;
  position: relative !important;
  padding-left: 50px;
  min-width: 600px;
}
.roam-main {
  width: unset !important;
  max-width: 100% !important;
  height: 100%;
  overflow-x: scroll;
  overflow-y: hidden;
  margin: auto;
  transition: padding-left 0.15s ease-out;
}

.block-highlight-blue {
background-color: var(--color-primary-highlight) !important;
z-index: 99;
}

div::selection, textarea::selection {
background-color: var(--color-primary-highlight);
}

/* Typography */
h1, h2, h3, h4, h5, h6, .rm-level1, .rm-level2, .rm-level3 .rm-title-editing-display {
  font-family: var(--header-font);
}
.rm-title-editing-display textarea {
  font-family: var(--header-font);
  font-size: 1em;
}
div, textarea {
  font-family: var(--body-font);
  font-size: var(--font-size);
  color: var(--text-color);
}
.roam-block-container {
  max-width: 1000px;
}



/* Embed Blocks */
.rm-embed-container {
  background: #fcfdfd;
  border: 1px solid var(--color-subtle-border);
  border-radius: 4px;
  padding: 0.6em 0.4em;
  margin: 0.4em 0;
}
.block-highlight-yellow {
  background-color: white;
}
/* Code Syntax */
code {
  font-family: var(--code-font);
  background: #F0F4F8;
  color: var(--text-color);
  border: none;
  padding: 4px 6px;
  opacity: 90%;
}

/* Queries */
.rm-query {
  border: 0.5px solid #e4e9ec;
  border-radius: 5px;
}
.rm-query .rm-query-title {
  background-color: #f7f8f8;
  padding: 0.8em;
  color: #d1dbe2;
  font-size: 80%;
}
.rm-reference-main.rm-query-content {
  padding: 0.8em;
}
.rm-reference-main, .rm-reference-item {
  font-size: 95%;
  opacity: 95%;
}
.rm-ref-page-view-title span {
}
.rm-reference-main .rm-reference-item .controls {
  margin-left: -1em;
}
.rm-ref-page-view {
  padding: 0.4em 0.2em;
}
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page {
  padding: 6px;
}
div.flex-v-box.starred-pages-wrapper > div.flex-h-box > span {
  font-size: 14px;
  opacity: 80%;
  letter-spacing: 0.04em;
}
div.roam-sidebar-container.noselect > div > div {
  font-size: 14px;
  letter-spacing: 0.03em;
}
#block-input {
  background: white;
}
.roam-body #block-input > span > div {
  padding: 6px 24px;
  background: white;
}

.rm-block-text, .roam-block {
  max-width: 64ch;
  font-size: 1.1em;
  line-height: 1.6em;
}
#right-sidebar > div {
  background-color: white;
  border-left: 1px solid #e9ebef;
  padding: 20px;
  overflow: none;
}
.rm-page-ref-brackets {
  display: none;
}


/* Bullet Points */
.rm-bullet .rm-bullet__inner {
box-sizing: content-box;
  display: flex;
  align-items: center;
  overflow: hidden;
  border-radius: 50%;
  width: 5px;
  height: 5px;
  background-clip: content-box;
  border: 4px solid transparent;
  background-color: #E3ECF2;
}

.rm-bullet.rm-bullet--closed .rm-bullet__inner {
  box-sizing: content-box;
  border: 4px solid #D8E5EE;
}


.block-border-left {
  border-left: 1px solid #fff;
}
.kanban-board {
  background-color: #fff;
}
.kanban-card {
  background-color: white;
  margin: 8px;
  box-shadow: 0px 1px 2px #9eb3c0;
  padding: 10px;
  border-radius: 2px;
  line-height: 1.3em;
}
.kanban-title {
  text-align: center;
  font-weight: bold;
  padding-top: 6px;
}
.kanban-column {
  background-color: #e4edf2;
  margin: 0px 4px 0px 4px;
  padding: 4px;
  min-width: 200px;
  border-radius: 3px;
}
.rm-block-ref::before {
  content:"";
  display: inline-block;
  width: 2px;
  border-radius: 2px;
  height: 10px;
  background: var(--color-primary-light);
  margin-right: 6px;
}
.rm-block-ref:hover {
  background: none;
  cursor: pointer;
}

.rm-block-ref {
  border-bottom: none;
  font-size: 1em;
  color: var(--text-color);
  opacity: 90%;
}
.block-ref-count-button {
  color: var(--color-primary);
  font-weight: 800;
  top: -10px;
}
.checkmark {
  background: #fff;
}
.check-container input:checked ~ .checkmark {
  background: #33bdea;
}
.check-container input:checked ~ .checkmark:after {
  border-color: #fff;
}
.rm-reference-item {
  margin-top: 8px;
  border-radius: 6px;
  border: 1px solid #e4e9ee;
  margin-right: 8px;
  flex: 1 1 100%;
  word-break: break-word;
  background-color: #f7f9fb;
  padding: 8px;
}
.rm-level1 div, .rm-level1 textarea {
  font-size: 1.7rem;
  font-weight: 600;
}
.rm-level2 div, .rm-level2 textarea {
  font-size: 1.4rem;
}
.rm-level3 div, .rm-level3 textarea {
  color: var(--light-text-color);
  font-weight: 400;
  font-size: 1.3rem;
}
a {
 color: var(--color-secondary);
font-weight: 600;
}
.intercom-app, .intercom-launcher-frame, #intercom-container {
  display: none;
}
.roam-body .roam-app .roam-sidebar-container {
  background-color: white;
  border-right: 1px #eee solid;
}
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page, .roam-body .roam-app .roam-sidebar-container > * {
  opacity: 80%;
  box-shadow: none;
}
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page:hover, .roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button:hover {
  background: white;
  color: black;
  opacity: 100%;
}
#buffer.tall {
  height: calc(100vh - 50px);
}
.check-container {
  padding-right: 4px;
}
span.rm-page-ref {
  border-radius: 2px;
  padding-left: 1px;
  padding-right: 1px;
}

.center-proj {
  text-align: center;
}
.rm-alias-external, .rm-alias-external:hover {
  font-weight: 600;
}

/* Set the colour of popover tooltip text to white */
.bp3-tooltip .bp3-popover-content div {
color: white;
}

/* Page Link and Tag Colours */

.rm-page-ref--tag {
  color: var(--page-tag-color);
}
.rm-page-ref--link {
  color: var(--color-primary);
  font-weight: 600;
}




/* -------------------------- */

/* Custom Data Tags and Pages */

/* -------------------------- */
span.rm-page-ref[data-tag="Tweet"], span[data-link-title^="Tweet"] .rm-page-ref {
  background: #81d5ed !important;
  color: white !important;
  padding: 3px 7px;
  line-height: 2em;
  font-weight: 500;
}
span.rm-page-ref[data-tag="Literature Notes"], span[data-link-title^="Literature Notes"] .rm-page-ref {
  background: #9769ff !important;
  color: white !important;
  padding: 3px 7px;
  font-weight: 500;
  line-height: 2em;
}
span.rm-page-ref[data-tag="Evergreens"], span[data-link-title^="Evergreens"] .rm-page-ref {
  background: #0dbac6 !important;
  color: #fff !important;
  padding: 3px 8px;
  line-height: 2em;
  font-weight: 500;
}
span.rm-page-ref[data-tag="Seedling"], span[data-link-title^="Seedling"] .rm-page-ref {
  color: #0dbac6 !important;
  padding: 2px;
  font-weight: 600;
  line-height: 1.4em;
  font-size: 0.7em;
  vertical-align: 10%;
  opacity: 80%;
}
span.rm-page-ref[data-tag="Idea Bank"], span[data-link-title^="Idea Bank"] .rm-page-ref {
  color: #fcb815 !important;
  padding: 3px 4px;
  font-weight: 700;
  line-height: 1.4em;
}
span.rm-page-ref[data-tag="Idea Bank"]:before {
  content:"✦ ";
}
span.rm-page-ref[data-tag="core"], span[data-link-title^="Idea Bank"] .rm-page-ref {
  color: #fcb815 !important;
  padding: 3px 4px;
  font-weight: 700;
  line-height: 1.4em;
}
span.rm-page-ref[data-tag="core"]:before {
  content:"✦ ";
}
span.rm-page-ref[data-tag="Illustrated Notes"], span[data-link-title^="Illustrated Notes"] .rm-page-ref {
  color: #7172fc;
  padding: 3px 4px;
  font-weight: 700;
  line-height: 1.4em;
}
span.rm-page-ref[data-tag="Garden Notes"], span[data-link-title^="Garden Notes"] .rm-page-ref {
  color: #9dbc13;
  padding: 3px 4px;
  font-weight: 700;
  line-height: 1.4em;
}
span.rm-page-ref[data-tag="Video Tutorial"] {
  color: #db3b8d;
  padding: 3px 4px;
  line-height: 1.4em;
  font-weight: 700;
}
span.rm-page-ref[data-tag="Essay"], span[data-link-title^="Essay"] .rm-page-ref {
  background: #adcb2a;
  color: #fff;
  padding: 3px 7px;
  line-height: 2em;
  font-weight: 500;
}
span.rm-page-ref[data-tag="Livestream"], span[data-link-title^="Livestream"] .rm-page-ref {
  color: #b979cf;
  padding: 3px 4px;
  line-height: 1.4em;
  font-weight: 700;
}
span.rm-page-ref[data-tag="Talk"], span[data-link-title^="Talk"] .rm-page-ref {
  background: #7172fc;
  color: #fff;
  padding: 3px 7px;
  line-height: 2em;
  font-weight: 500;
}
span.rm-page-ref[data-tag="waiting-for"], span[data-link-title^="Waiting"] .rm-page-ref {
  background: #f9c866;
  color: #fff;
  padding: 3px 7px;
  line-height: 2em;
  font-weight: 500;
}
span.rm-page-ref[data-tag="Researching"], span[data-link-title^="Researching"] .rm-page-ref {
  background: #ff9d66 !important;
  color: #fff;
  padding: 3px 7px;
  line-height: 2em;
  font-weight: 500;
}
span.rm-page-ref[data-tag="Synthesising"], span[data-link-title^="Synthesising"] .rm-page-ref {
  background: #fc766f !important;
  color: #fff !important;
  padding: 3px 7px;
  line-height: 2em;
  font-weight: 500;
}
span.rm-page-ref[data-tag="Alive"], span[data-link-title^="Alive"] .rm-page-ref {
  background: #ee5f85 !important;
  color: #fff !important;
  padding: 3px 7px;
  line-height: 2em;
  font-weight: 500;
}
span[data-link-title^="Book/"] .rm-page-ref {
  color: #119bf0 !important;
  font-weight: 600;
}
span[data-link-title^="Evergreen/"] .rm-page-ref {
  color: #00acc0 !important;
  font-weight: 600;
}
span[data-link-title^="➽"] .rm-page-ref {
  color: #35b2d4 !important;
  font-weight: 700;
}
span[data-link-title^="Video/"] .rm-page-ref {
  color: #119bf0 !important;
  font-weight: 600;
}
span[data-link-title^="Project/"] .rm-page-ref {
  color: #4CAF50 !important;
  font-weight: 700;
}
span[data-link-title^="Area/"] .rm-page-ref {
  color: #d4357f !important;
  font-weight: 600;
}
span[data-link-title^="Article/"] .rm-page-ref {
  color: #119bf0 !important;
  font-weight: 600;
}
span[data-link-title^="Course/"] .rm-page-ref {
  color: #5391f8 !important;
  font-weight: 600;
}
span[data-link-title^="Idea/"] .rm-page-ref {
  color: #fcb815 !important;
  padding: 3px 4px;
  font-weight: 700;
  line-height: 1.4em;
}
span[data-link-title^="Idea/"] .rm-page-ref::before {
  content:"✦ ";
}


/* -------------------------- */

/* Block Styles by Tag */

/* -------------------------- */


.roam-block-container[data-page-links*='Claim'] {
  background: #FDF8EE;
  border-radius: 6px;
  padding: 0.6em 0.4em 0.4em 0em;
}

 span.rm-page-ref[data-tag="Claim"], span[data-link-title^="Claim"] .rm-page-ref {
   opacity: 70%;
   font-size: 80%;
   color: #FFC585;
}

.roam-block-container[data-page-links*='Questions'] {
  background: #ECF5FB;
  border-radius: 6px;
  padding: 0.6em 0.4em 0.4em 0em;
}

span.rm-page-ref[data-tag="Questions"], span[data-link-title^="Questions"] .rm-page-ref {
   opacity: 70%;
   font-size: 80%;
   color: #91B9E5;
}

.roam-block-container[data-page-links*='Response'] {
  background: #F3F1FD;
  margin-top: 2px;
  border-radius: 6px;
  padding: 0.6em 0.4em 0.4em 0em;
}

 span.rm-page-ref[data-tag="Response"], span[data-link-title^="Response"] .rm-page-ref {
   opacity: 70%;
   font-size: 80%;
   color: #AFA0E1;
}

.roam-block-container[data-page-links*='Evidence'] {
  background: #FEEDED;
  margin-top: 2px;
  border-radius: 6px;
  padding: 0.6em 0.4em 0.4em 0em;
}

 span.rm-page-ref[data-tag="Evidence"], span[data-link-title^="Evidence"] .rm-page-ref {
   opacity: 70%;
   font-size: 80%;
   color: #F99292;
}

.roam-block-container[data-page-links*='DirectQuote'] {
  background: #F4F6D8;
  margin-top: 2px;
  border-radius: 6px;
  padding: 0.6em 0.4em 0.4em 0em;
}

 span.rm-page-ref[data-tag="DirectQuote"], span[data-link-title^="DirectQuote"] .rm-page-ref {
   opacity: 70%;
   font-size: 80%;
   color: #A5C16A;
}```
