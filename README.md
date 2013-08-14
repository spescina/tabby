# Tabby
Tabby is a lightweight JavaScript and CSS kit for mobile-first toggle tabs. It's style-light so you can easily modify it to fit your design.


## Basic Tabs
Turn any set of `<a>` or `<button>` elements into tabs by wrapping them in a `<div>` with the `.tabs` class. Assign each tab a `data-target` whose value matches the ID of the tab content.

Wrap all tab content `<div>` elements for a particular tab set in `<div>` with the `.tabs-content` class.

    <div class="tabs">
        <button data-target="#tab1">Superheroes</button>
        <button data-target="#tab2">Ice Cream</button>
        <button data-target="#tab3">Seasons</button>
    </div>

    <div class="tabs-content">
        <div class="tabs-pane active" id="tab1">
            Superheros
            ...
        </div>

        <div class="tabs-pane" id="tab2">
            Ice Cream
            ...
        </div>

        <div class="tabs-pane" id="tab3">
            Seasons
            ...
        </div>
    </div>


## Horizontal Tabs
Styled navigation that displays horizontally.

Add the `.active` class to the current `<li>` in the navigation to apply special styling.

    <ul class="tabs tabs-horizontal">
        <li class="active"><a data-target="#tab1" href="#">Superheroes</a></li>
        <li><a data-target="#tab2" href="#">Ice Cream</a></li>
        <li><a data-target="#tab3" href="#">Seasons</a></li>
    </ul>

    <div class="tabs-content">
        <div class="tabs-pane active" id="tab1">
            Superheros
            ...
        </div>

        <div class="tabs-pane" id="tab2">
            Ice Cream
            ...
        </div>

        <div class="tabs-pane" id="tab3">
            Seasons
            ...
        </div>
    </div>


## Stacked Navigation
On smaller screens, stacked tabs mimic the appearance of horizontal tabs. On bigger screens, navigation appears in a vertical stack next to the content.

This demo uses the grid system from [Kraken](http://cferdinandi.github.io/kraken/). Feel free to use whatever grid you prefer.

    <div class="row">
        <div class="grid-2">
            <div class="tabs">
                <li class="active"><a data-target="#tab1" href="#">Superheroes</a></li>
                <li><a data-target="#tab2" href="#">Ice Cream</a></li>
                <li><a data-target="#tab3" href="#">Seasons</a></li>
            </div>
        </div>
        <div class="grid-4">
            <div class="tabs-content">
                <div class="tabs-pane active" id="tab1">
                    Superheros
                    ...
                </div>

                <div class="tabs-pane" id="tab2">
                    Ice Cream
                    ...
                </div>

                <div class="tabs-pane" id="tab3">
                    Seasons
                    ...
                </div>
            </div>
        </div>
    </div>


## Progressively Enhanced
By default, tab navigation is hidden and all tab content is visible.

Tabby includes a script that checks for JavaScript support by adding a `.js` class to the `<body>` on page load. This activates Tabby, showing the tabs and hiding tab content.

That way, people without JavaScript support still have access to the content.


## Browser Support
Tabby works on all modern browsers, and IE 8 and above. Tabby also requires [jQuery](http://jquery.com/).


## Changelog
* v2.1 (August 5, 2013)
  * Updated with variable for `$(this)` (better performance).
* v2.0 (June 7, 2013)
  * Switched to MIT license.
* v2.0 (June 5, 2013)
  * Switched from `href` to `data-target` value for tab id, breaking backward compatibility.
* v1.1 (February 13, 2013)
  * Renamed `example.html` to `index.html`.
* v1.1 (February 5, 2013)
  * Switched to relative sizing.
* v1.0 (January 22, 2013)
  * Initial release.


## License
Tabby is free to use under the [MIT License](http://gomakethings.com/mit/).
