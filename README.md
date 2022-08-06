# 1. RUN
```
git clone https://github.com/raijp/node.git
cd node
docker-compose up -d --build
```

JSX to JS
```
#docker exec -it node1-v1.0 mkdir -p www/react
#docker exec -it node1-v1.0 mkdir -p www/react/js_src/js
#docker exec -it node1-v1.0 mkdir -p www/react/js_dst/js
#docker exec -it node1-v1.0 npm i -D --prefix ./www/react @babel/cli
#docker exec -it node1-v1.0 npm i -D --prefix ./www/react @babel/core
#docker exec -it node1-v1.0 npm i -D --prefix ./www/react @babel/preset-react
#docker exec -it node1-v1.0 /bin/bash -c 'echo {\"presets\":[\"@babel/preset-react\"]} > ./www/react/.babelrc'
# add scripts to package.js

docker exec -it node1-v1.0 npm --prefix ./www/react/ run cmp
```
