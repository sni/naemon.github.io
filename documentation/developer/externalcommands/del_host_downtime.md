---
layout: default
title: External Command Reference
---

<!--
************************************************
* AUTO GENERATED PAGE - USE ./update SCRIPT
************************************************
-->

<span class="glyphicon glyphicon-arrow-up"></span><a href="index.html"> External Commands Reference</a> - DEL_HOST_DOWNTIME<br>


#### Command Format:

`DEL_HOST_DOWNTIME;downtime_id`

#### Description:

Deletes the host downtime entry that has an ID number matching the 'downtime_id' argument. If the downtime is currently in effect, the host will come out of scheduled downtime (as long as there are no other overlapping active downtime entries).

#### Shell Script Usage Example:

```sh
#!/bin/sh
# This is a sample shell script showing how you can submit the DEL_HOST_DOWNTIME command
# to Naemon. Adjust variables to fit your environment as necessary.

printf "[%lu] DEL_HOST_DOWNTIME;1234\n" `date +%s` > /var/lib/naemon/naemon.cmd
```



