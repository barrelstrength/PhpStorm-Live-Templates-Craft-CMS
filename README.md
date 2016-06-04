# PhpStorm Live Templates for Craft CMS

A library of PhpStorm Live Templates for Craft CMS. 

The **Craft CMS** Live Templates include various snippets for Craft-specific Twig tags and some other common use cases. Best when paired with [Twig - Extended](https://github.com/BarrelStrength/PhpStorm-Live-Templates-Twig-Extended) - a more extensive library of PhpStorm Live Templates for Twig.

## Twig

### Craft Twig Tags (via tab trigger)

The following tab triggers output a simple example of a loop in two different formats for their respective Craft tags. The first trigger, provides an example using chaining syntax (craft.entries.section('articles')). The second trigger with the same name ending with `o`, provides the same example using object syntax.

    asset                    craft.assets.first()
    assets, assetso          craft.assets loop
    categories, categorieso  craft.categories loop
    entries, entrieso        craft.entries loop
    feed                     craft.feeds.getFeedItems loop
    tags, tagso              craft.tags loop
    users, userso            craft.users loop

    cache                    {% cache %}...{% endcache %}
    children                 {% children %}
    exit                     {% exit 404 %}
    ifchildren               {% ifchildren %}...{% endifchildren %}
    includecss               {% includecss %}...{% endincludecss %}
    includecssfile           {% includeCssFile "/resources/css/global.css" %}
    includehirescss          {% includehirescss %}...{% endincludehirescss %}
    includejs                {% includejs %}...{% endincludejs %}
    includejsfile            {% includeJsFile "/resources/css/global.css" %}
    matrix, matrixif         Basic Matrix field loop using if statements
    matrixifelse             Basic Matrix field loop using if/elseif
    matrixswitch             Basic Matrix field loop using switch
    nav                      {% nav item in items %}...{% endnav %}
    paginate                 Outputs example of pagination and prev/next links
    redirect                 {% redirect 'login' %}
    requirelogin             {% requireLogin %}
    requirepermission        {% requirePermission "spendTheNight" %}
    switch                   {% switch variable %}...{% endswitch %}

    // Output Helpers
    csrf                     {{ getCsrfInput() }}
    getFootHtml              {{ getFootHtml() }}
    getHeadHtml              {{ getHeadHtml() }}

    // craft.request
    getparam                 craft.request.getParam()
    getpost                  craft.request.getPost()
    getquery                 craft.request.getQuery()
    getsegment               craft.request.getSegment()

    // Closing tags
    case                     {% case "value" %}
    endcache                 {% endcache %}
    endifchildren            {% endifchildren %}
    endincludecss            {% endincludecss %}
    endincludehirescss       {% endincludehirescss %}
    endincludejs             {% endincludejs %}
    endnav                   {% endnav %}

### Craft Twig Functions (via tab trigger)

    ciel                     ceil()
    floor                    floor()
    max                      max()
    min                      min()
    round                    round()
    shuffle                  shuffle()
    url, urla                url('path'), url('path', params, 'http', false)

## PHP

### Migrations (via tab trigger)

    migrate                  A basic migration class

### Debugging (via tab trigger)

    dd                       Craft::dd("Dump & Die");

----

## Installation

Copy the `Craft CMS.xml` file to the location where PhpStorm stores Live Templates on your operating system. The PhpStorm docs provide [instructions on installing Live Templates](https://www.jetbrains.com/help/phpstorm/10.0/live-templates.html) on OSX, Windows, and Linux.

Visit `Preferences->Editor->Live Templates` and ensure that the **Craft CMS** Live Templates are enabled.

----

## Maintenance & Contributions

If you'd like to contribute to the **Craft CMS** Live Templates, please consider submitting a pull request, reporting an issue, providing examples of how you would like to see the behavior of the Live Templates improved, or just sending your thoughts.

## References

- [Craft CMS](https://craftcms.com/)
- [Twig](http://www.twig-project.org/)
- [PhpStorm](https://www.jetbrains.com/phpstorm/)
- [PhpStorm Live Templates for Twig](https://github.com/BarrelStrength/PhpStorm-Live-Templates-Twig-Extended) - A more extensive library of PhpStorm Live Templates for Twig.
- [Straight Up Craft](https://straightupcraft.com)
