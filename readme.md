# gr-mx

## What is this repository ?
This is a repository of scripts and results to check Greek ISPs' mail servers TLS support for SMTP.

## Read More
[The sorry state of STARTTLS support of Greek email providers](https://www.void.gr/kargig/blog/2016/01/23/the-sorry-state-of-starttls-support-of-greek-email-providers/)

[Update on the state of STARTTLS support of Greek email providers](https://www.void.gr/kargig/blog/2016/03/26/update-on-the-state-of-starttls-support-of-greek-email-providers/)


## Current status

Status according to the latest results file.

| Commercial Provider | CA or Self Signed | Max TLS version  |
|:--------------------|:-----------------:| ----------------:|
| COSMOTE             | CA-signed         |              1.2 |
| Wind                | CA-signed         |              1.2 |
| Cyta                | CA-signed         |              1.2 |
| Forthnet            | CA-signed         |              1.2 |
| HOL                 | NO CERTIFICATE    |              N/A |
| Vodafone            | CA-signed         |              1.2 |

| Non-Commercial Provider | CA or Self Signed | Max TLS version  |
|:------------------------|:-----------------:| ----------------:|
| GRNET                   | CA-signed         |              1.2 |
| SCH                     | NO CERTIFICATE    |              N/A |
| TEE                     | CA-signed         |              1.2 |
| MIL                     | Self-signed       |              1.2 |

| Universities | CA or Self Signed | Max TLS version  |
|:-------------|:-----------------:| ----------------:|
| AUTH         | CA-signed         |              1.2 |
| NTUA         | CA-signed         |              1.2 |
| UPATRAS      | CA-signed         |              1.0 |

| Free Providers | CA or Self Signed | Max TLS version  |
|:---------------|:-----------------:| ----------------:|
| IN             | NO CERTIFICATE    |              N/A |
| FREEMAIL       | CA-signed         |              1.2 |
| MAILBOX        | CA-signed         |              1.2 |

| Radical Providers | CA or Self Signed | Max TLS version  |
|:------------------|:-----------------:| ----------------:|
| Espiv             | CA-signed         |              1.2 |

For details regarding the certificates of each ISP read the blog posts.

## How to run the scripts on your own

run the script
```
# ./mx-script | tee results/results-`date +%Y%m%d`
```


see which MX servers support STARTTLS
```
# grep TLS results/results-`date +%Y%m%d`
```
