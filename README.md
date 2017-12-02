## Overview

Wrapper for the `ifstat` command that outputs JSON objects.

## Installation

```
npm install -g ifstat-json
```

## Usage

No options at this time; Only the simple script is available.
```
$ ifstat-json
```

## Details

The script outputs JSON objects that are in the following format ( interface names are dynamically grabbed ):
```
{ hostname: 'Roberts-MBP',
  date: 2017-12-02T06:33:25.694Z,
  interfaces: 
   { lo0: { in: 0, out: 0 },
     gif0: { in: 0, out: 0 },
     stf0: { in: 0, out: 0 },
     en0: { in: 0.98, out: 0.33 },
     en1: { in: 0, out: 0 },
     en2: { in: 0, out: 0 },
     p2p0: { in: 0, out: 0 },
     awdl0: { in: 0, out: 0 },
     bridge0: { in: 0, out: 0 } } }
```

Note that the output is actually all on a single line, and looks like the following:
```
{"hostname":"Roberts-MBP","date":"2017-12-02T06:33:25.694Z","interfaces":{"lo0":{"in":0,"out":0},"gif0":{"in":0,"out":0},"stf0":{"in":0,"out":0},"en0":{"in":0.98,"out":0.33},"en1":{"in":0,"out":0},"en2":{"in":0,"out":0},"p2p0":{"in":0,"out":0},"awdl0":{"in":0,"out":0},"bridge0":{"in":0,"out":0}}}
```
