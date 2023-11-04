# strong_type
`build2` package for the [`strong_type`](https://github.com/rollbear/strong_type) C++ library.

Note: This is the source code for the build2 package of the `strong_type` C++ library, the actual library sources snapshot can be found in the ./upstream/ submodule.

## Usage

You can simply add this package as dependency to your project by specifying it in your `manifest`:

```
depends: strong_type ^12.0.0
```

Then just pick the targets that you need:

```
import libs  = strong_type%lib{strong_type}
```

Make sure to add the stable section of the cppget.org repository to your project's repositories.manifest to be able to fetch the package.

```
:
role: prerequisite
location: https://pkg.cppget.org/1/stable
# trust: ...
```
