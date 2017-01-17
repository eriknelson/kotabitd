# About

`kotabit` is my attempt at porting [greyhole](https://www.greyhole.net/) to golang.

`kotabitd` is the [kotabit](https://github.com/eriknelson/kotabit) cli. Project
is organized as a library driven by this project.
See [golang wiki](https://github.com/golang/go/wiki/GithubCodeLayout)

# Prerequisites

[glide](https://github.com/Masterminds/glide) is used for better locked down and
sandboxed package management. It is akin to a bundler or npm. It must be installed
to `$PATH` or otherwise available.

`glide install` from the project directory should get you up and running on the
cli.

# Development

It's recommended for ongoing development to link in the separate kotabit
libraries to the vendor projects so changes to the library are picked up
on subsequent builds. `scripts/glide-link` and `scripts/glide-unlink` are
helpers for this purpose.

```
go get github.com/eriknelson/kotabit
./scripts/glide-link github.com/eriknelson/kotabit
```
