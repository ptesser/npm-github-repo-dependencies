# NPM Packages from GitHub repository

## Public repository

I tried the flow with a **public** repository using this source: https://github.com/ptesser/ng-form

I run `npm install --save ptesser/ng-form#master`.

It has generated the above code:

```JSON
{
  "dependencies": {
    "ng-form": "github:ptesser/ng-form#master"
  }
}
```

## Private repository

I tried the flow with a **private** repository using a dump.




## References

- https://medium.com/@jonchurch/use-github-branch-as-dependency-in-package-json-5eb609c81f1a
- https://martinwolf.org/2018/04/github-branch-as-dependency-package-json/