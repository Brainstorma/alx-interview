# 0x03-log_parsing

## Description

This project parses web server logs and generates metrics from the data.

## 0-stats.py

This script parses web server logs from stdin and generates metrics from the log data.

It prints statistics about:

- Total file size transferred
- Total number of status codes returned  
- List of IP addresses accessed and number of times accessed
- List of HTTP status codes returned and number of times returned

Usage:


* The script should print statistics about the total file size transferred and the total number of status codes returned

### 1. Log parsing - extended

* Based on the previous task, extend the log parsing script to print statistics about:

  - Total file size transferred

  - Number of status codes returned

  - List of IPs accessed and number of times accessed 

  - List of HTTP status codes returned and number of times returned

* Print statistics in a human-readable format

### 2. Log parsing - cutting fields

* Based on the previous task, update the script to extract fields from each log line using `cut`:

  - The IP field

  - The date field

  - The request field 

  - The status code field

  - The file size field

* Print the extracted fields for each log line while parsing the log

## Usage

The script can be run like:

```bash
$ ./0-generator | ./0-stats.py
```

## Tasks To Complete

+ [x] 0. **Log parsing**<br/>[0-stats.py](0-stats.py) contains a script that reads `stdin` line by line and computes metrics:
  + Input format: `<IP Address> - [<date>] "GET /projects/260 HTTP/1.1" <status code> <file size>` (if the format is not this one, the line must be skipped).
  + After every 10 lines and/or a keyboard interruption (`CTRL + C`), print these statistics from the beginning:
    + Total file size: `File size: <total size>`.
    + Where `<total size>` is the sum of all previous `<file size>` (see input format above)
    + Number of lines by status code:
      + Possible status code: `200`, `301`, `400`, `401`, `403`, `404`, `405` and `500`.
      + If a status code doesn’t appear or is not an integer, don’t print anything for this status code.
      + Format: `<status code>: <number>`.
      + Status codes should be printed in ascending order.

