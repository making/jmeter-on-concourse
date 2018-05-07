
```
cp credentials.yml.sample credentials.yml
fly -t ci sp -p jmeter -c pipeline.yml -l credentials.yml
fly -t ci tj -j jmeter/perf-test --watch
```