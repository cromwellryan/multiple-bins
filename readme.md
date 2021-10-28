## Working with multiple binaries in an npm package...


You can provide multiple binaries in an npm package. You can do this 
explicitly, like this silly repo does. You can also use [`directors.bin`](https://docs.npmjs.com/cli/v7/configuring-npm/package-json#directoriesbin)


To test this out:

```
git clone git@github.com:cromwellryan/multiple-bins.git
npm install -g ./multiple-bins
echo "bin1 is available in PATH at $(which bin1)"
echo "bin2 is available in PATH at $(which bin2)"
npm uninstall -g multiple-bins
```

Finally, run `bin1` and `bin2` to see that both are available. `which bin1` and `which bin2` will give you insight too.
