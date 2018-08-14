## References

This configuration was created using https://github.com/looplab/logspout-logstash


## Usage

Logsout will collect logs from a single docker machine, thus this container must be started from the docker-host. 

### On Windows with docker toolbox, using WSL, connect to the host with the following command:

```
#Connect to docker machine
docker-machine ssh default
```

Then use the following commands to start logspout

```
git clone https://github.com/nvankaam/logspout.git
cd logspout
docker-compose up -d
```

The docker-compose file contains configuration where to send the logs. The default configuration will send it to localhost.