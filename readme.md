# Simple New Relic Installation

`To Install newrelic you need New Relic Account and API Key`

After you create your account, go to API Keys and create one if you don't already have.

## Update Machine

```
sudo apt update
```

## Installing New Relic and PHP Agent

```
curl -Ls https://download.newrelic.com/install/newrelic-cli/scripts/install.sh | bash && sudo NEW_RELIC_API_KEY=<API_KEY> NEW_RELIC_ACCOUNT_ID=<ACCOUNT_ID> /usr/local/bin/newrelic install -n php-agent-installer
```
Above command line will install newrelic cli and php agent

#### To Install Only newrelic cli:

```
curl -Ls https://download.newrelic.com/install/newrelic-cli/scripts/install.sh | bash && sudo NEW_RELIC_API_KEY=<API_KEY> NEW_RELIC_ACCOUNT_ID=<ACCOUNT_ID> /usr/local/bin/newrelic install
```

## Another Way

`APM > Add more Data > Select the Application Language` and follow on screen instructions.