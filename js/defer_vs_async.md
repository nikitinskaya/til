# Async vs defer

- both only work with external scripts
- if async and defer attributes are placed together, only async will work in modern browsers, and only defer in IE9-
- the page continues to load while the script is loading
- if added dynamically with a function, ```script.async = false;``` ensures the right order of scripts execution (they still load simultaneously though). Without this, scripts default to async

| async  | defer  |
|:---:|:---:|
| ie9+  | all browsers  |
| doesn't wait for all page to load, starts executing  |   waits for all doc to be ready, then executes|
|  the first script to load is the first to run | strict script order, top-down, used if second script depends on the first one  |

