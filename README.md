# Worldcup Slack Bot

WorldCupBot will notify a Slack channel/group for every matches during the 2018 FIFA World Cup Russia™.

It uses the "unofficial" FIFA json API (the one used for their mobile apps).

It will post a message :
  - when a match starts
  - for every red/yellow card
  - for the half time and end time
  - and of course, for every goal

### Preview

Here is a preview of the Colombia vs Japan match.

![worldcup-slack-bot sample](https://i.imgur.com/H5kUavh.png)

### Requirements

  - PHP >= 5.3
  - You need a token from Slack:
    - Jump at https://api.slack.com/custom-integrations/legacy-tokens (you have to login)
    - and you will find your token.

### Installation

  - Clone this repo
  - Set up a cron to run every minute:

  ````
  * * * * * cd /path/to/folder && php worldCupNotifier.php >> worldCupNotifier.log
  ````

### Side notes

The code is ugly but it works.

Everything is posted in french, but feel free to fork and use your own language. FYI, FIFA API can provide text in en/fr/de/es/pt.

### Want a Docker image? 

Try out  ![docker image](https://hub.docker.com/r/okram999/fifa2018-slackbot/) 
