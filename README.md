## Ruby

* For compare two array

```ruby
arr1 = [1, 2, 3, 4, 5]
arr2 = [5, 6, 7, 8, 9]
arr3 = [10, 11, 12, 13, 14]

(arr1 & arr2).empty? # => false
(arr1 & arr3).empty? # => true
```

## Ruby on Rails
* For disable generate assets, test views, helpers
[https://gist.github.com/dimasjt/a621b7f8ce9f25906e9e601e9291df8d](https://gist.github.com/dimasjt/a621b7f8ce9f25906e9e601e9291df8d)


## PosgreSQL

* Import data
```bash
  $ psql -U postgres_user -d database_name -a -f data.sql
```

## MeteorJS

* Cross Origin Cors, add this code in server directory
```javascript
WebApp.connectHandlers.use(function(req, res, next) {
  res.setHeader("Access-Control-Allow-Origin", "*");
  return next();
});

```

## Atom.io

- [Highlight selected](https://atom.io/packages/highlight-selected)
- [Emmet](https://atom.io/packages/emmet)
- [git-diff-details](https://atom.io/packages/git-diff-details)
- [Ruby slim](https://atom.io/packages/ruby-slim)