## The loaded JS

* Quick intro, we only have 15 minutes, and I bet you're not here to see me.

* Some baseline info:

JS is loaded two at a time.

Loading scripts (but not just scripts) blocks the entire UI from rendering until
they're loaded.

(Hence loading them at the bottom of the page)

(But that only helps you in a page scenario, not an app)

* But… there’s gotta be a better way!

* Enter defer/async.

Tag attributes which modify how JS is loaded. Add the attribute, boom, job done.

* defer

Defer automates this task which people have been doing since the 90s:

$(document).ready(function() { … });

It'll load the JS, but `defer` its execution until the DOM is ready.

"cool story bro image"

* async

`async` is `defer`'s the tricky cousin. It'll do what `defer` does, except it'll fire execution as soon as it's loaded.

Useful for stuff like analytics code, and things that aren't paramount for the
functioning of the app.

* Does this replace the need for loaders?

Err, no. Application code loading requires logic.

E.g.: When module x is loaded, do Y.

These attributes just give you more control over how JS is loaded.

* Demonstrate loading times and scenarios.

* Show support tables from caniuse.

* Thanks.
