# ScrapeSend
Scrapes a website and sends a group text message message

Uses `nohup` requests to send automated updates via SMS at a daily scheduled time that run as background processes
**IMPORTANT:** as `nohup` requests run as background process code termination or system shutdown will not terminate the process
To terminate a `nohup` process you must first find all running process by typing the following on your terminal:
```
ps -ef
```
The process ID should be listed on the second column. To terminate the process enter:
```
kill "process ID"
```
where `process ID` is the given ID

### Example:
The current code scrapes `mortgagenewsdaily.com` and sends daily updated mortgage rates to a list of subscribers
