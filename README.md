# NativeScript documentation

Welcome to the NativeScript documentation content repository. The documentation site is generated by [Jekyll](https://jekyllrb.com/), and this repository hosts the page content and related assets.

## Multiple configurations

We have two Jekyll builds for the documentation that generate similar output: `nativescript` and `angular`. The former builds the vanilla NativeScript docs, while the latter discusses Angular2-specific topics. Most of the content is shared between the two, and several options are available to add environment-specific content:

1. Pages that appear in certain environment only. Adding an `environment: angular` to a page's front matter will mark that page as being available only in that environment. Other environment builds will exclude it. Pages not marked with `environment` will be shared across all environments.

2. Display different content on shared pages. This is possible via our environment-related block tags, named `angular` and `nativescript` respectively:
    ```
    {% nativescript %}Dependency properties...{% endnativescript %}

    {% angular %}Change detection...{% endangular %}[
    ```
