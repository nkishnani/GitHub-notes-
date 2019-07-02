# Useful Tools

### `cron`

The `cron` Unix utility allows you to automate tasks that are needed to be run on a schedule. This becomes especially useful when dealing with system administration. When working at [CareerVillage.org](careervillage.org) I found a lot of use cases for `cron`. For example, emails are sent out every day to mentors recommending questions for them to answer. This task would be trivial for a software engineer to do, so we outsourced it to the `cron` utility to run within our docker container (hosted on AWS).
