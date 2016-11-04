## HowTo

- exposing ports is only needed for testsing
- simulation-client accesses exposed ports via docker network

`docker build -t simulation-server .`

`docker run --rm -ti --name=simulation-server -p 3001:3001 -p 3002:3002 -p 3011:3011 -p 3022:3022 \
        simulation-server`