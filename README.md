# 1. RUN
```
git clone https://github.com/raijp/node.git
cd node
docker-compose up -d --build
```

JSX to JS
```
#docker exec -it node1-v1.0 mkdir -p babel/react
#docker exec -it node1-v1.0 npm i -D --prefix ./babel/react babel-cli
#docker exec -it node1-v1.0 npm i -D --prefix ./babel/react babel-core
#docker exec -it node1-v1.0 npm i -D --prefix ./babel/react babel-preset-react
#docker exec -it node1-v1.0 /bin/bash -c 'echo {\"presets\":[\"react\"]} > ./babel/react/.babelrc'
# add scripts to package.js

docker exec -it node1-v1.0 npm --prefix ./babel/react/ run cmp-dir
```
