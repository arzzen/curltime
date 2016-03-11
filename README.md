### Bash cUrl time

A command line tool to measure HTTP request time with cUrl.

Measure single HTTP request time or average time of multiple requests.

#### Usage

> ./curltime.sh [url] [attempts]

#### Example:

Command (default attempts = 1):

`$ ./curltime.sh http://www.github.com`

or with attempts

`$ ./curltime.sh http://www.github.com 5`

Output:

<pre>
 Url:	www.github.com

 +-----------------------------------------------------------------------------------+
 | #       |                           Time (seconds)                                |
 +-----------------------------------------------------------------------------------+
 | Attempt | Connect | Start transfer | Redirect | Namelookup | Pretransfer |  Total |
 +-----------------------------------------------------------------------------------+
 | 1.      |   0.061 |          0.289 |    0.000 |      0.061 |       0.061 |  0.290 |
 | 2.      |   0.005 |          0.232 |    0.000 |      0.004 |       0.005 |  0.232 |
 | 3.      |   0.005 |          0.229 |    0.000 |      0.004 |       0.005 |  0.229 |
 | 4.      |   0.005 |          0.235 |    0.000 |      0.004 |       0.005 |  0.236 |
 | 5.      |   0.005 |          0.233 |    0.000 |      0.004 |       0.005 |  0.234 |
 +-----------------------------------------------------------------------------------+
 | summary |   0.016 |          0.243 |        - |          - |           - |  0.244 |
 +-----------------------------------------------------------------------------------+
</pre>
