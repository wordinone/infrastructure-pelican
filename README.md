# Tools for using Pelican at the ASF

_TBD_

## Step One: Build libcmark-gfm

```
$ sudo apt install cmake g++
$ mkdir /tmp/cm
$ cd /tmp/cm
$ /path/to/infrastructure-pelican/bin/build-cmark.sh
... (build output here)
export LIBCMARKDIR='/tmp/cm/cmark-gfm-0.28.3.gfm.12/lib'
$
```

Copy/paste/execute that printed `export` line for use in the following steps.

(of course, you may use any location of your choice; `/tmp/cm` is
merely an example)

### Installing libcmark-gfm via packages

_TBD: install a .deb from packages.apache.org_

_TBD: maybe a macOS variant?_

_TBD: maybe Windows?_

## Step Two

_TBD: credentials need to provided in (eg.) bb2.txt_

```
$ ./kick_build.py --repo=www-site --notify=somewhere@example.com --theme theme/apache --min-pages=200
```
