# yoga-layout

> Prebuilt for Windows

Prebuilt JS version of the yoga layout flexbox engine.

## Usage with `@react-pdf/renderer`

`package.json`

```
{
  "dependencies": {
    "yoga-layout-prebuilt": "github:rayyee/yoga-layout-windows-2G",
    "@react-pdf/renderer": "latest"
  }
}
```

This will override the `yoga-layout` dependency of `react-pdf` and so it can
be installed on Windows as well.

See these issues for the current status [react-pdf](https://github.com/diegomura/react-pdf/issues/151) and [yoga](https://github.com/facebook/yoga/issues/411).
