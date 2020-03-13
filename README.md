# XcodeSupportScripts
 Make Xcode convenient with custom scripts

# Add Scripts

- Save under following scripts to any location.

- Open Behaviors

```
Xcode > Preference > Behaviors Tab
```

- Save a any script and any custom script 

# Scripts

## Open Terminal

Open current github repository as terminal

```
#!/bin/bash
open -a Terminal "`pwd`"
```

## Open github repository page with chrome

Open current github repository as chrome


```
#!/bin/bash
pwd | git remote -v | grep fetch | awk '{print $2}' | xargs open -a '/Applications/Google Chrome.app'
```

