## Silverstripe CMS kitchen sink recipe

[![CI](https://github.com/silverstripe/recipe-kitchen-sink/actions/workflows/ci.yml/badge.svg)](https://github.com/silverstripe/recipe-kitchen-sink/actions/workflows/ci.yml)

The kitchen sink is an internal recipe used for testing the full Silverstripe CMS feature sets,
including optional and suggested modules.

## Get started

You can create a project using Composer:

```
composer create-project silverstripe/recipe-kitchen-sink ./cms-sink ^4
```

## More information

See the [recipe plugin](https://github.com/silverstripe/recipe-plugin) page for instructions on how
Silverstripe CMS recipes work.

## Troubleshooting

### Page and PageController parent classes

When installing the kitchen sink, your project Page and PageController subclasses may be set to extend
SiteTree and ContentController. This is [only an issue](https://github.com/silverstripe/cwp-recipe-kitchen-sink/issues/30)
with the kitchen sink recipe, and requires you to manually change the parent classes to CWP's BasePage and
BasePageController.
