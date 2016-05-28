# Assetic extensions bundle

[![Build Status](https://img.shields.io/travis/IncSW/AsseticExtensionsBundle/master.svg?style=flat-square)](https://travis-ci.org/IncSW/AsseticExtensionsBundle)

## Configuration
```yaml
incsw_assetic_extensions:
    filters:
        babel:
            config: %kernel.root_dir%/../.babelrc
```

## Examples
### Babel filter
````twig
{% javascripts '@AppBundle/Resources/public/js/*' filter='babel' %}
    <script src="{{ asset_url }}"></script>
{% endjavascripts %}
````

## License
[MIT](https://github.com/IncSW/AsseticExtensionsBundle/blob/master/LICENSE)
