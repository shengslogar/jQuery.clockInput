jQuery.clockInput
====================

Introduction
------------

Transforms `<input type="time">` into a pretty, circular clock. Keep using your input the way you would! **ClockInput** binds itself
to the original input element, preventing you from having to change
any existing code.

Shiny.

Requirements
------------
-   jQuery


Usage
-----

One line. Boom.

    $("input[type=time]").clockInput();
    
Notes
-----

This plugin currently only supports the following native attributes of
an `input type=time` input (rounds to nearest five minutes for all values):

- `min` - Minimum time selectable (24hh:mm)
- `max` - Maximum time selectable (24hh:mm)
- `value` - Currently selected time (24hh:mm)

Tip: add `autocomplete="off"` to time inputs in Firefox to prevent input caching on page
reload.

Bugs
----
To file a bug report, please send an email to
[slogar.sheng@gmail.com](mailto:slogar.sheng@gmail.com?subject=jQuery.clockInput+Bug+Report).

Todos
----
This was originally built specifically around a client's requirements.
Potential contributions/future todos could look like:

- Accessibility baby (tabs, arrow keys, etc.)
- Customizable minute increments (supporting corresponding `step` attrib)
- 12/24 hour mode
- Add time button that magically adds 2 hours of daylight
  to your current physical day
- Improved, more intuitive animations
- Free coffee

Version History
---------------
0.0.2

-   Fixed issue parsing input `value` attribute in Firefox.
    Other minor fixes/improvements. (20171110)

0.0.1

-   Fixed min/max time bounds issue (when maxhour == minhour), added console error message on invalid bound params,
    slightly tweaked styles (20171019)
-   Minor tweaks, added webkit support for kicks (20170420)
-   Initial version. Expect plump bugs (20170420)


License
---------------------

This work is licensed under the
[Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).