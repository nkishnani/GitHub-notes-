# Useful Tools

### `cron`

The `cron` Unix utility allows you to automate tasks that are needed to be run on a schedule. This becomes especially useful when dealing with system administration. When working at [CareerVillage.org](careervillage.org) I found a lot of use cases for `cron`. For example, emails are sent out every day to mentors recommending questions for them to answer. This task would be trivial for a software engineer to do, so we outsourced it to the `cron` utility to run within our docker container (hosted on AWS).



The main paradigm when working with `cron` is the `cron` table, often shortened to `crontab`.

- `crontab -l` : lists the current jobs in the `cron` table
- `crontab -e` : allows you to edit the `cron` table, in the default text editor (likely `vim`)



```bash
# ┌───────────── minute (0 - 59)
# │ ┌───────────── hour (0 - 23)
# │ │ ┌───────────── day of the month (1 - 31)
# │ │ │ ┌───────────── month (1 - 12)
# │ │ │ │ ┌───────────── day of the week (0 - 6) (Sunday to Saturday;
# │ │ │ │ │                                   7 is also Sunday on some systems)
# │ │ │ │ │
# │ │ │ │ │
# * * * * * command to execute
```

So, for example:

- ` * * * * * echo "Hello, World!" >> /Desktop/test.txt` will print `"Hello, World!"` into the given file *every* minute of *every* hour of *every* day, and so on and so forth.
- `0 9 1 * * python3 script.py` will run the `script.py` at 9AM every 1st of the month.





