# electrumx-docker
Dockerfile for [electrumx](https://github.com/kyuupichan/electrumx) on Ubuntu with leveldb and daemontools.

## Usage
### Configuration
```
git clone https://github.com/followtheart/electrumx-docker.git
cd electrumx-docker
```

Edit `env/DAEMON_URL` to match your AXE core settings.

### Run
Run from docker hub:
```shell
    docker run -v env:/env  -idt axerunners/electrumx
```

Or build your special env docker image :
```shell
      docker build -t electrumx .
      docker run -v -idt electrumx
```

Based on https://github.com/followtheart/electrumx-docker
