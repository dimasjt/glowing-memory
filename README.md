## Ruby

For compare two array

```ruby
arr1 = [1, 2, 3, 4, 5]
arr2 = [5, 6, 7, 8, 9]
arr3 = [10, 11, 12, 13, 14]

(arr1 & arr2).empty? # => false
(arr1 & arr3).empty? # => true
```
