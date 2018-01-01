# Dependencies
```
git
docker
docker-compose
```

# Setup
```bash
$ git clone git@github.com:D-Dawg/msStack.git
$ git submodule init
$ git submodule update
```

You might want to link your local mongodb data with the docker db
```bash
$ ln -s /var/lib/mongodb mongodb/db
```
Might not work on every system.

**Alternative:** Move local mongodb (`/var/lib/mongodb` on linux) to `./mongodb/db` ]

or use a empty db and restore db dump.

```bash
$ git clone git@github.com:D-Dawg/msTourism2.git
$ docker-compose up  #[-d = detach]
```
## memory problem
error: max virtual memory areas vm.max_map_count [65530] is too low, increase to at least [262144]
```bash
sysctl -w vm.max_map_count=262144
```
