# Django REST Swagger

[![build-status-badge]][build-status]
[![pypi-version]][pypi]
[![license-badge]][license]
[![docs-badge]][docs]

####An API documentation generator for Swagger UI and Django REST Framework

This project is built on the [Django REST Framework Docs](https://github.com/marcgibbons/django-rest-framework-docs) and uses the lovely [Swagger from Wordnik](https://developers.helloreverb.com/swagger/) as an interface. This application introspectively generates documentation based on your Django REST Framework API code. Comments are generated in combination from code analysis and comment extraction. Here are some of the features that are documented:

* API title - taken from the class name
* Methods allowed
* Serializers & fields in use by a certain method
* Field default values, minimum, maximum, read-only and required attributes
* URL parameters (ie. /product/{id})
* Field `help_text` property is used to create the description from the serializer or model.

## Requirements
* Python (2.6.5+, 2.7, 3.2, 3.3, 3.4)
* Django (1.5.5+, 1.6, 1.7)
* Django REST framework (2.3.5+)

## Bugs & Contributions
Please report bugs by opening an issue

Contributions are welcome and are encouraged!

## Django settting for egg loader

```python
TEMPLATE_LOADERS = (
    'django.template.loaders.filesystem.Loader',
    'django.template.loaders.app_directories.Loader',
    'django.template.loaders.eggs.Loader',
)
```

## Special Thanks
Thanks to [BNOTIONS](http://www.bnotions.com) for sponsoring initial development time.

Many thanks to Tom Christie & all the contributors who have developed [Django REST Framework](http://django-rest-framework.org/)

## Contributors
* Marc Gibbons (@marcgibbons)
* Geraldo Andrade (@quein)
* Vítek Pliska (@whit)
* Falk Schuetzenmeister (@postfalk)
* Lukas Hetzenecker (@lukas-hetzenecker)
* David Wolever (@wolever)
* Brian Moe (@bmoe)
* Ian Martin (@aztechian)
* @pzrq
* @jfelectron
* Warnar Boekkooi (@boekkooi)
* Darren Thompson (@WhiteDawn)
* Lukasz Balcerzak (@lukaszb)
* David Newgas (@davidn)
* Bozidar Benko (@bbenko)
* @pySilver


### Django REST Framework Docs contributors:

* Scott Mountenay (@scottmx81)
* @swistakm
* Peter Baumgartner (@ipmb)
* Marlon Bailey (@avinash240)


[build-status-badge]: https://travis-ci.org/marcgibbons/django-rest-swagger.svg?branch=master
[build-status]: https://travis-ci.org/marcgibbons/django-rest-swagger
[pypi-version]: https://pypip.in/version/django-rest-swagger/badge.svg
[pypi]: https://pypi.python.org/pypi/django-rest-swagger
[license-badge]: https://pypip.in/license/django-rest-swagger/badge.svg
[license]: https://pypi.python.org/pypi/django-rest-swagger/
[docs-badge]: https://readthedocs.org/projects/django-rest-swagger/badge/
[docs]: http://django-rest-swagger.readthedocs.org/
