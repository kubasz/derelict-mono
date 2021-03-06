DerelictMono
============
[![Dub version](https://img.shields.io/dub/v/derelict-mono.svg)](https://code.dlang.org/packages/derelict-mono)

Dynamic and static bindings to version 5.0 of the [Mono Runtime][1] for the D Programming Language. It can be used for [embedding][2] a Common Language Runtime in D.

Please see the pages [Building and Linking Derelict][3] and [Using Derelict][4], in the Derelict documentation, for information on how to build DerelictMono and load Mono at run time. Please also look at [DerelictGLFW3 documentation][5] to see how to use the static bindings, the subconfiguration is named `derelict-mono-static`. In the meantime, here's some sample code.

```D
import derelict.mono.mono;

void main()
{
    // Load the Mono library.
    DerelictMono.load();

    // Now Mono functions can be called.
    ...
}
```

[1]: http://www.mono-project.com/
[2]: http://www.mono-project.com/docs/advanced/embedding/
[3]: http://derelictorg.github.io/compiling.html
[4]: http://derelictorg.github.io/using.html
[5]: https://derelictorg.github.io/packages/glfw3.html
