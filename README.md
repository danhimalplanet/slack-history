# save history of slack channel to csv file

clone repo

install golang

``brew install golang``

get Slack token

set SLACK_TOKEN environment variable (put a space before 'export' to keep it out of your shell history)

`` export SLACK_TOKEN="xoxb-24530992559-48910202342365-MFkc2sadfguHKm5GGOj5YSGfg4s"``

save contents of 'cats' channel from 2011-04-18 till now to a csv file.  the csv file name will be the slackID of the channel

``go run slack-history.go -start 2011-04-18T00:00:00Z -channel "cats"``
