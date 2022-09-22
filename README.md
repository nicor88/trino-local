# trino-local
A simple setup to get start with trino.

## Requirements
* Docker Runtime

## Getting started
To run trino simply run: `make trino-up`. If everything works sucessfully you can reach trino coordinator UI at [localhost:8080](http://localhost:8080).
In order to connect to trino and run your first query you have 2 options:
* Install a client like Dbeaver and connect via it
* Run `make trino-cli` then run this query `SELECT count(*) FROM tpch.tiny.nation;` if you get a result everything worked fine


## Notes
* The sum of `query.max-memory-per-node`  and `memory.heap-headroom-per-node` cannot be bigger than the maxHeapSize
