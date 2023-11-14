## What is this

A simple cjs wrapper to the forked [change-case](https://github.com/olsonpm/change-case/tree/fix-ems-compatible/packages/change-case) module

Here is [the original module](https://github.com/blakeembrey/change-case)

## Why make a wrapper ?

Since version 5 of change-case, the module [only supports esm import](https://github.com/blakeembrey/change-case/issues/305#issuecomment-1745124038).
In order to continue using this module conveniently I decided to fork it and wrap it in [fix-esm](https://www.npmjs.com/package/fix-esm).

## Why isn't change-case declared as a peer dependency ?

Unfortunately change-case uses [package.json -> exports](https://nodejs.org/api/packages.html#exports)
which prevents fix-esm from working as normal.  This is why I forked it.  The
fork should be very easy to keep up-to-date.
