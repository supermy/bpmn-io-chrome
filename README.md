# bpmn-js packaged as a chrome app

This project embeds and packages [bpmn-js](https://github.com/bpmn-io/bpmn-js) as a chrome app and makes available locally.


## Build

#### Package + Run

```
grunt
```

```
chrome --load-and-launch-app="$(pwd)/dist" resources/simple.bpmn
```

#### Development Setup

```
grunt auto-build
```



### Integration


#### A simple binary

(put to `/usr/local/bin` or the like)

```bash
#!/bin/bash

APP_DIR=path-to/bpmn-js-chrome/dist

chrome --load-and-launch-app="$APP_DIR" $@
```

Execute it as

```
bpmn-io foo.bpmn
```