# NPM Packages from GitHub repository

## Public repository

I tried the flow with a **public** repository using this source: https://github.com/ptesser/ng-form

- Run `npm install --save ptesser/ng-form#master`.

It has generated the above code:

```JSON
{
  "dependencies": {
    "ng-form": "github:ptesser/ng-form#master"
  }
}
```

## Private repository

I tried the flow with a **private** repository using a dumb source code.

- Generate a GitHub token with `repo` scaope
- Insert the follow line inside `package.json`
- Run `npm install`

`"<package-name>": "git+https://<generated-token>:x-oauth-basic@github.com/<user-name>/<repo-name>.git#<branch-name>"
`

## Note

This trick could be achieve only with repositories that have the `package.json` file.

## References

- http://nts.strzibny.name/using-private-github-repositories-with-yarn-and-npm-in-package-json/
- https://medium.com/@jonchurch/use-github-branch-as-dependency-in-package-json-5eb609c81f1a
- https://martinwolf.org/2018/04/github-branch-as-dependency-package-json/
