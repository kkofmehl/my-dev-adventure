# Sql Server DevOps

## Speaker

Scott Sauber

Slides at scottsauber.com

## Notes:

- 77% of devs are responsible for database and application development

- "You can't change culture and process with a credit card."

- DBAs tend to think we are trying to replace them, when in fact it's just getting rid of a mundane part of their job.


## What Choices do I need to make?

## What are the tradeoffs?

## What tools are out there?

## What hurdles will I face?

## Migration-based approach

- Every change in scripted
- Scripts are commited to source control
- Scripts run in order
- Which scripts have run are kept track in a table
- Write them up front during dev
- Run the same scripts in every env

## How?

- DB Code and App Code should live together in the same repo

## Flyway

- Open Source

## RedGate Sql Migration

- Enterprise $$$

## Rollbacks
- They are ussally not worth the headache

