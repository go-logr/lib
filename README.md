# lib

A collection of helper packages that work with any go-logr implementation.

Allowed dependencies in this module are the Go standard library and
github.com/go-logr/logr. The same Go versions as in github.com/go-logr/logr are
supported. This ensures that all code which uses logr can also use this module.

logr itself must not depend on the "lib" module to avoid a dependency
cycle. Helper code needed by logr must be in the logr module.
