## Examples

{% tabs %}
{% tab label="Simple Library" %}

Creates the `my-ui-lib` library with an `ui` tag:

```bash
nx g @nrwl/angular:library my-ui-lib --tags=ui
```

{% /tab %}

{% tab label="Nested Folder & Import"%}
Creates the `my-lib` library in the `nested` directory and sets the import path to `@myorg/nested/my-lib`:

```bash
nx g @nrwl/angular:library --directory=nested --importPath=@myorg/nested/my-lib my-lib
```

{% /tab %}

{% tab label="Standalone component"%}
Creates the `my-standalone-lib` library with a standalone component as an entry point instead of an ng-module. The component can be used via the `myorg-standalone-component` selector.

```bash
nx g @nrwl/angular:library --standalone --selector=myorg-standalone-component  my-standalone-lib
```

{% /tab %}
