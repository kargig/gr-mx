# gr-mx

## What is this repository ?
This is a repository of scripts and results to check Greek ISPs' mail servers TLS support for SMTP.

## Read More
[The sorry state of STARTTLS support of Greek email providers](https://www.void.gr/kargig/blog/2016/01/23/the-sorry-state-of-starttls-support-of-greek-email-providers/)

[Update on the state of STARTTLS support of Greek email providers](https://www.void.gr/kargig/blog/2016/03/26/update-on-the-state-of-starttls-support-of-greek-email-providers/)


## Current status

Status according to the latest results file.

| Commercial Provider | CA or Self Signed | Max TLS version  | Supports SSLv3 |
|:--------------------|:-----------------:| ----------------:|---------------:|
| COSMOTE             | CA-signed         |          1.0/1.2 |         Yes/No |
| Wind                | CA-signed         |          1.0/1.2 |         Yes/No |
| Cyta                | CA-signed         |              1.2 |             No |
| Forthnet            | CA-signed         |              1.2 |             No |
| HOL                 | NO CERTIFICATE    |              N/A |            N/A |
| Vodafone            | CA-signed         |              1.2 |             No |

| Non-Commercial Provider | CA or Self Signed | Max TLS version  | Supports SSLv3 |
|:------------------------|:-----------------:| ----------------:|---------------:|
| GRNET                   | CA-signed         |              1.2 |             No |
| SCH                     | NO CERTIFICATE    |              N/A |            N/A |
| TEE                     | CA-signed         |              1.2 |         Yes/No |
| MIL                     | Self-signed       |              1.2 |             No |

| Universities | CA or Self Signed | Max TLS version  | Supports SSLv3 |
|:-------------|:-----------------:| ----------------:|---------------:|
| AUTH         | CA-signed         |              1.2 |            Yes |
| NTUA         | CA-signed         |              1.2 |            Yes |
| UPATRAS      | CA-signed         |              1.0 |            Yes |

| Free Providers | CA or Self Signed | Max TLS version  | Supports SSLv3 |
|:---------------|:-----------------:| ----------------:|---------------:|
| IN             | NO CERTIFICATE    |              N/A |            N/A |
| FREEMAIL       | CA-signed         |              1.2 |             No |
| MAILBOX        | CA-signed         |              1.2 |             No |

| Radical Providers | CA or Self Signed | Max TLS version  | Supports SSLv3 |
|:------------------|:-----------------:| ----------------:|---------------:|
| Espiv             | CA-signed         |              1.2 |             No |

For details regarding the certificates and supported TLS versions of each provider read the blog posts.

## How to run the scripts on your own

run the script
```
# ./mx-script | tee results/results-`date +%Y%m%d`
```


see which MX servers support STARTTLS
```
# grep TLS results/results-`date +%Y%m%d`
```
