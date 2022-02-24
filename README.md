1. Look in `libs/lib-buildable/project.json` - notice how there is a `build:random-config` configuration
2. Now look in `apps/shell/project.json` - notice the `dependsOn` config
3. Run `nx build shell -c random-config` - it will print `Cannot find configuration 'random-config' for project 'shell:build'`
4. Expected behavior: it should allow the build, use the default configuration for Shell, and pass the `random-config` to its `lib-buildable` dependencygi
