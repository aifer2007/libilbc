Changes in 2.0.1 (2014-12-11)
-----------------------------

- Update to r7765, cc7755b.
- Fix crash in programs directly calling Init functions, without first
  creating a context through constructors.
- Proper SONAME versioning added, and bumped to libilbc.so.2.

Changes in 2.0.0 (2014-11-17)
-----------------------------

- Under new maintainership by me (Timothy Gu).
- Update to latest upstream source (r7715, 087da13).
  - A threading implementation is now needed. Win32 and POSIX Threads are
    supported.
- Autotools files are cleaned-up.
- CMake now uses BUILD_SHARED_LIBS to determine the type of library to build.
- CMake installation paths on some 64-bit systems using `lib64/` are
  corrected.
- Git metadata for merging from upstream is added for easier merging.
- Travis CI support is added.