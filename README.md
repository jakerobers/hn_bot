
parse-hn returns Hacker News in the format `url		title` (tab delimited)

irc-push will send content from stdin and disconnect. This makes it cron-friendly

```
wget https://news.ycombinator.com | ./parse-hn | ./irc-push --host="yourhostname" --port="6667" --nick="hackernewsbot" --channel="yourchannelname"
```
