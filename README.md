# yoga-layout

`2GB = 2147483648 bytes`, But use the value of `2147483647` on 64-bit arch   
[https://nodejs.org/api/buffer.html#buffer_buffers_and_typedarray](https://nodejs.org/api/buffer.html#buffer_buffers_and_typedarray)
> Allocates a new Buffer of size bytes. If size is larger than [buffer.constants.MAX_LENGTH](https://nodejs.org/api/buffer.html#buffer_buffer_constants_max_length) or smaller than 0, [ERR_INVALID_OPT_VALUE](https://nodejs.org/api/errors.html#ERR_INVALID_OPT_VALUE) is thrown. A zero-length Buffer is created if size is 0.   

> On 32-bit architectures, this value is (2^30)-1 (~1GB). On 64-bit architectures, this value is (2^31)-1 (~2GB).


## Prebuilt for Windows

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
