# Testing GraphQL in Browser
An example of loading GraphQL in browser and using it for querying game data intuitively.
```gql
self {
	nearestBuilding(target:"campfire", distanceLessThan:5, inVision:true) {
		distance
		position
		pathTo
	}
}
```

## Building GraphQL.js
```sh
# install rollup
npm install --global rollup
# clone and build graphql npm package
git clone https://github.com/graphql/graphql-js
cd graphql-js
npm install
npm run build:npm
# package graphql library in a single bundle
cd npmDist
rollup index.mjs --format umd --name "graphql" --file ../../graphql.bundle.js
```

License for graphql bundle can be found here: https://github.com/graphql/graphql-js?tab=MIT-1-ov-file#readme

