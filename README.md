# PhpStorm Live Templates for Craft CMS

Twig and PHP PhpStorm Live Templates for Craft CMS 3.

The **Craft CMS** Live Templates include various snippets for Craft-specific Twig tags and some other common use cases. Best when paired with [Twig - Extended](https://github.com/BarrelStrength/PhpStorm-Live-Templates-Twig-Extended) - a more extensive library of PhpStorm Live Templates for Twig.

## Craft CMS - Twig

### Craft Twig Tags (via tab trigger)

    // Examples
    asset                    craft.assets.first()
    assets                   craft.assets loop
    categories               craft.categories loop
    entries                  craft.entries loop
    feed                     craft.feeds.getFeedItems loop
    matrix, matrixif         Basic Matrix field loop using if statements
    matrixifelse             Basic Matrix field loop using if/elseif
    matrixswitch             Basic Matrix field loop using switch
    paginate                 Outputs example of pagination and prev/next links
    tags                     craft.tags loop
    users                    craft.users loop

    // Output Helpers
    cache                    {% cache %}...{% endcache %}
    csrf                     {{ csrfInput() }}
    children                 {% children %}
    exit                     {% exit 404 %}
    ifchildren               {% ifchildren %}...{% endifchildren %}
    hook                     {% hook "$NAME$" %}
    nav                      {% nav item in items %}...{% endnav %}
    redirect                 {% redirect 'login' %}
    redirectinput            {{ redirectInput($URL$) }}
    requirelogin             {% requireLogin %}
    requirepermission        {% requirePermission "spendTheNight" %}
    switch                   {% switch variable %}...{% endswitch %}

    css                      {% css %}...{% endcss %}
    js                       {% js %}...{% endjs %}
    registercssfile          {% do view.registerCssFile("css/style.css") %}
    registerjsfile           {% do view.registerJsFile("js/script.js") %}

    header                   {% header "string" %}
    beginBody                {{ beginBody() }}
    endbody                  {{ endBody() }}
    head                     {{ head() }}

    // Closing tags
    case                     {% case "value" %}
    endcache                 {% endcache %}
    endifchildren            {% endifchildren %}
    endcss                   {% endcss %}
    endjs                    {% endjs %}
    endnav                   {% endnav %}

    // craft.app
    app                      craft.app.[CURSOR]
    config                   craft.app.config.general.[CURSOR]
    ismultisite              craft.app.isMultiSite
    language                 craft.app.language
    locale                   craft.app.locale

    // craft.app.request
    getparam                 craft.app.request.getParam("name")
    getbodyparam             craft.app.request.getBodyParam("name")
    getqueryparam            craft.app.request.getQueryParam("name")
    getsegment               craft.app.request.getSegment(1)

    // craft.app.i18n
    alllocales               craft.app.i18n.allLocales
    applocales               craft.app.i18n.appLocales
    editablelocaleids        craft.app.i18n.editableLocaleIds
    editablelocales          craft.app.i18n.editableLocales
    getlocalebyid            craft.app.i18n.getLocaleById($ID$)
    primarysitelocale        craft.app.i18n.primarySiteLocale
    sitelocaleids            craft.app.i18n.siteLocaleIds
    sitelocales              craft.app.i18n.siteLocales

### Craft Twig Functions (via tab trigger)

    alias                    alias("@baseUrl/images/image.png")
    ceil                     ceil()
    classname                className(object)
    clone                    clone(object)
    floor                    floor()
    getenv                   getenv('name')
    max                      max()
    min                      min()
    round                    round()
    shuffle                  shuffle()
    svg                      svg('path')
    url, urla                url('path'), url('path', params, 'https', false)
    siteurl, siteurla        siteUrl('path'), siteUrl('path', params, 'https', 1)

## Craft CMS - PHP

### Migrations (via tab trigger)

    migrate                  A basic migration class

### Debugging (via tab trigger)

    dd                       Craft::dd("Dump & Die");

----

## Installation

 1. Download and enable the Settings Repository Plugin: *PhpStorm Preferences | Plugins | Settings Repository*
 2. Go to *PhpStorm Preferences | Tools | Settings Repository*
 3. Add Read-only Source https://github.com/barrelstrength/PhpStorm-Live-Templates-Craft-CMS
 4. Restart PhpStorm

Visit `Preferences->Editor->Live Templates` and ensure that the **Craft CMS - Twig** and **Craft CMS - PHP** Live Templates are enabled, as desired.

- Craft CMS - Twig.xml
- Craft CMS - PHP.xml

----

## Maintenance & Contributions

If you'd like to contribute to the **Craft CMS** Live Templates, please consider submitting a pull request, reporting an issue, providing examples of how you would like to see the behavior of the Live Templates improved, or just sending your thoughts.

## References

- [Craft CMS](https://craftcms.com/)
- [Twig](http://www.twig-project.org/)
- [PhpStorm](https://www.jetbrains.com/phpstorm/)
- [PhpStorm Live Templates for Twig](https://github.com/BarrelStrength/PhpStorm-Live-Templates-Twig-Extended) - A more extensive library of PhpStorm Live Templates for Twig.
- [Straight Up Craft](https://straightupcraft.com)
