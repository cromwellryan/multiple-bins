## Working with multiple binaries in an npm package...


You can provide multiple binaries in an npm package. You can do this 
explicitly, like this silly repo does. You can also use [`directors.bin`](https://docs.npmjs.com/cli/v7/configuring-npm/package-json#directoriesbin)


To test this out, clone it to a path. Then, in another directory, run `npm install -g <folder path>`

Finally, run `bin1` and `bin2` to see that both are available. `which bin1` and `which bin2` will give you insight too.
