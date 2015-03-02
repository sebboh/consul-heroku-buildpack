# Heroku Buildpack for Consul

This is a simple buildpack for running Consul agent on Heroku

## Usage

add `--buildpack https://github.com/sebboh/consul-heroku-buildpack` when creating your Heroku application

After deploying, run the Consul agent with `heroku ps:scale consul=1`

The buildpack currently runs a test agent. You'll need to modify the start command in bin/release to do something more meaningful with the agent.
