# gr-mx

## What is this repository ?
This is a repository of scripts and results to check Greek ISPs' mail servers TLS support for SMTP.

## Read More
[The sorry state of STARTTLS support of Greek email providers](https://www.void.gr/kargig/blog/2016/01/23/the-sorry-state-of-starttls-support-of-greek-email-providers/)
[Update on the state of STARTTLS support of Greek email providers](https://www.void.gr/kargig/blog/2016/03/26/update-on-the-state-of-starttls-support-of-greek-email-providers/)

## How to run the scripts on your own

run the script
```
# ./mx-script | tee results/results-`date +%Y%m%d`
```


see which MX servers support STARTTLS
```
# grep TLS results/results-`date +%Y%m%d`
```
