# Crontab



```
crontab -> allows to schedule the execution of scripts
-l      -> show crontab list
-e      -> edit the crontab table. With this more scripts can be added
```

```bash
0   16  *   *   *    $Home/src/cronjobs/daily.sh
0   *   *   *   *    $Home/src/cronjobs/hourly.sh
*   *   *   *   *    $Home/src/cronjobs/minutely.sh
```

Columns:

1. minute 0-59
2. hour 0-23
3. day month 1-31
4. moth 1-12
5. day week: 0-7 (0 & 7 sunday)
6. script/command

**Example 1 (for the minute column)**

```
1       -> runs in minute 1  
1,10,18 -> runs at minute 1, 10 and 18  
`*/5    -> runs every 5 minutes  
1-10    -> runs the first 10 minutes of every hour  
*       -> runs every minute
```

**Example 2**

```bash
*/15 4 * * * script.sh
```

Run script.sh:

* every day of the week
* every month
* every day of the month
* at 4 am
* every 15 minutes

**Example 3**

```bash
0 3 * * 1 script.sh
```

Run script.sh:

* only if it's monday
* every month
* every day of the month
* at 3 am
* at minute zero

**Note**: when editing the crontab table, make sure the columns are sorted
