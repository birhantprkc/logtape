---
links:
  '#215': https://github.com/dahlia/logtape/issues/215
  '#216': https://github.com/dahlia/logtape/pull/216
---
 -  Added the `rotatedFilePath` option to `getRotatingFileSink()` to customize
    rotated log file paths, for example to keep the *.log* extension.
    [[#215], [#216]]

 -  Changed `getRotatingFileSink()` to reject positive `maxFiles` values unless
    they are integers from 1 to 1,000, throwing `RangeError` during sink
    creation. Update configurations outside this range before upgrading.  Zero
    and negative values still disable backups.  [[#216]]
