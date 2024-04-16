# security-hub-aggregator

A tool that aggregate findings from AWS Security Hub.

## Architecture

![architecture](./resources/architecture.drawio.png)

## Work Flow

![workflow](./resources/stepfunctions_graph.png)

## Deployment

If you had already installed AWS SAM, it's a only command below.

> sam deploy --guided

## Warning

- Be careful with a eventbridge's rule, because this tool may send too many messages.
  - It may lead to overcharging especialy AWS Step Functions.
