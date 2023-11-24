---
title: "events(references)"
date : 2023-11-24
draft: true
---

# HTML Event Attributes

## Global Event Attributes

HTML memiliki kemampuan untuk membiarkan peristiwa memicu tindakan di browser, seperti memulai JavaScript ketika pengguna mengeklik sebuah elemen.

Di bawah ini adalah atribut event global yang dapat ditambahkan ke elemen HTML untuk mendefinisikan tindakan event.

## Jendela Atribut Event

Peristiwa yang dipicu untuk objek jendela (berlaku untuk tag <body>):

| Attribute | Value | Description |
| --- | --- | --- |
| [onafterprint](ev_onafterprint.asp) | _script_ | Script to be run after the document is printed |
| [onbeforeprint](ev_onbeforeprint.asp) | _script_ | Script to be run before the document is printed |
| [onbeforeunload](ev_onbeforeunload.asp) | _script_ | Script to be run when the document is about to be unloaded |
| [onerror](ev_onerror.asp) | _script_ | Script to be run when an error occurs |
| [onhashchange](ev_onhashchange.asp) | _script_ | Script to be run when there has been changes to the anchor part of the a URL |
| [onload](ev_onload.asp) | _script_ | Fires after the page is finished loading |
| onmessage | _script_ | Script to be run when the message is triggered |
| [onoffline](ev_onoffline.asp) | _script_ | Script to be run when the browser starts to work offline |
| [ononline](ev_ononline.asp) | _script_ | Script to be run when the browser starts to work online |
| onpagehide | _script_ | Script to be run when a user navigates away from a page |
| [onpageshow](ev_onpageshow.asp) | _script_ | Script to be run when a user navigates to a page |
| onpopstate | _script_ | Script to be run when the window's history changes |
| [onresize](ev_onresize.asp) | _script_ | Fires when the browser window is resized |
| onstorage | _script_ | Script to be run when a Web Storage area is updated |
| [onunload](ev_onunload.asp) | _script_ | Fires once a page has unloaded (or the browser window has been closed) |

## Form Events

Event yang dipicu oleh tindakan di dalam formulir HTML (berlaku untuk hampir semua elemen HTML, tetapi paling banyak digunakan dalam elemen formulir):

| Attribute | Value | Description |
| --- | --- | --- |
| [onblur](ev_onblur.asp) | _script_ | Fires the moment that the element loses focus |
| [onchange](ev_onchange.asp) | _script_ | Fires the moment when the value of the element is changed |
| [oncontextmenu](ev_oncontextmenu.asp) | _script_ | Script to be run when a context menu is triggered |
| [onfocus](ev_onfocus.asp) | _script_ | Fires the moment when the element gets focus |
| [oninput](ev_oninput.asp) | _script_ | Script to be run when an element gets user input |
| [oninvalid](ev_oninvalid.asp) | _script_ | Script to be run when an element is invalid |
| [onreset](ev_onreset.asp) | _script_ | Fires when the Reset button in a form is clicked |
| [onsearch](ev_onsearch.asp) | _script_ | Fires when the user writes something in a search field (for &lt;input="search"&gt;) |
| [onselect](ev_onselect.asp) | _script_ | Fires after some text has been selected in an element |
| [onsubmit](ev_onsubmit.asp) | _script_ | Fires when a form is submitted |

## Keyboard Events

| Attribute | Value | Description |
| --- | --- | --- |
| [onkeydown](ev_onkeydown.asp) | _script_ | Fires when a user is pressing a key |
| [onkeypress](ev_onkeypress.asp) | _script_ | Fires when a user presses a key |
| [onkeyup](ev_onkeyup.asp) | _script_ | Fires when a user releases a key |

## Mouse Events

| Attribute | Value | Description |
| --- | --- | --- |
| [onclick](ev_onclick.asp) | _script_ | Fires on a mouse click on the element |
| [ondblclick](ev_ondblclick.asp) | _script_ | Fires on a mouse double-click on the element |
| [onmousedown](ev_onmousedown.asp) | _script_ | Fires when a mouse button is pressed down on an element |
| [onmousemove](ev_onmousemove.asp) | _script_ | Fires when the mouse pointer is moving while it is over an element |
| [onmouseout](ev_onmouseout.asp) | _script_ | Fires when the mouse pointer moves out of an element |
| [onmouseover](ev_onmouseover.asp) | _script_ | Fires when the mouse pointer moves over an element |
| [onmouseup](ev_onmouseup.asp) | _script_ | Fires when a mouse button is released over an element |
| onmousewheel | _script_ | Deprecated. Use the [onwheel](ev_onwheel.asp) attribute instead |
| [onwheel](ev_onwheel.asp) | _script_ | Fires when the mouse wheel rolls up or down over an element |

## Geser Events

| Attribute | Value | Description |
| --- | --- | --- |
| [ondrag](ev_ondrag.asp) | _script_ | Script to be run when an element is dragged |
| [ondragend](ev_ondragend.asp) | _script_ | Script to be run at the end of a drag operation |
| [ondragenter](ev_ondragenter.asp) | _script_ | Script to be run when an element has been dragged to a valid drop target |
| [ondragleave](ev_ondragleave.asp) | _script_ | Script to be run when an element leaves a valid drop target |
| [ondragover](ev_ondragover.asp) | _script_ | Script to be run when an element is being dragged over a valid drop target |
| [ondragstart](ev_ondragstart.asp) | _script_ | Script to be run at the start of a drag operation |
| [ondrop](ev_ondrop.asp) | _script_ | Script to be run when dragged element is being dropped |
| [onscroll](ev_onscroll.asp) | _script_ | Script to be run when an element's scrollbar is being scrolled |

## Papan Klip Events

| Attribute | Value | Description |
| --- | --- | --- |
| [oncopy](ev_oncopy.asp) | _script_ | Fires when the user copies the content of an element |
| [oncut](ev_oncut.asp) | _script_ | Fires when the user cuts the content of an element |
| [onpaste](ev_onpaste.asp) | _script_ | Fires when the user pastes some content in an element |

## Media Events

Events yang dipicu oleh media seperti video, gambar, dan audio (berlaku untuk semua elemen HTML, tetapi paling umum terjadi pada elemen media, seperti `<audio>`, `<embed>`, `<img>`, `<object>`, dan `<video>`).

| Attribute | Value | Description |
| --- | --- | --- |
| onabort | _script_ | Script to be run on abort |
| oncanplay | _script_ | Script to be run when a file is ready to start playing (when it has buffered enough to begin) |
| oncanplaythrough | _script_ | Script to be run when a file can be played all the way to the end without pausing for buffering |
| oncuechange | _script_ | Script to be run when the cue changes in a &lt;track&gt; element |
| ondurationchange | _script_ | Script to be run when the length of the media changes |
| onemptied | _script_ | Script to be run when something bad happens and the file is suddenly unavailable (like unexpectedly disconnects) |
| onended | _script_ | Script to be run when the media has reach the end (a useful event for messages like "thanks for listening") |
| onerror | _script_ | Script to be run when an error occurs when the file is being loaded |
| onloadeddata | _script_ | Script to be run when media data is loaded |
| onloadedmetadata | _script_ | Script to be run when meta data (like dimensions and duration) are loaded |
| onloadstart | _script_ | Script to be run just as the file begins to load before anything is actually loaded |
| onpause | _script_ | Script to be run when the media is paused either by the user or programmatically |
| onplay | _script_ | Script to be run when the media is ready to start playing |
| onplaying | _script_ | Script to be run when the media actually has started playing |
| onprogress | _script_ | Script to be run when the browser is in the process of getting the media data |
| onratechange | _script_ | Script to be run each time the playback rate changes (like when a user switches to a slow motion or fast forward mode) |
| onseeked | _script_ | Script to be run when the seeking attribute is set to false indicating that seeking has ended |
| onseeking | _script_ | Script to be run when the seeking attribute is set to true indicating that seeking is active |
| onstalled | _script_ | Script to be run when the browser is unable to fetch the media data for whatever reason |
| onsuspend | _script_ | Script to be run when fetching the media data is stopped before it is completely loaded for whatever reason |
| ontimeupdate | _script_ | Script to be run when the playing position has changed (like when the user fast forwards to a different point in the media) |
| onvolumechange | _script_ | Script to be run each time the volume is changed which (includes setting the volume to "mute") |
| onwaiting | _script_ | Script to be run when the media has paused but is expected to resume (like when the media pauses to buffer more data) |

## Events Lainnya

| Attribute | Value | Description |
| --- | --- | --- |
| [ontoggle](ev_ontoggle.asp) | _script_ | Fires when the user opens or closes the &lt;details&gt; element |
