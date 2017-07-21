Buck shared library bug on macOS
================================

Try running

```
buck run //device:main
```

to reproduce. You should see a runtime error like

```
dyld: Library not loaded: @rpath/libopencv_videostab.3.2.dylib
  Referenced from: /.../buck-out/gen/device/main
  Reason: image not found
```
