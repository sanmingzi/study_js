# 循环

## for循环

```
function sum(begin, end) {
  var rtn = 0;
  for(var i = begin; i <= end; i++) {
    rtn += i;
  }
  return rtn;
}
console.log(sum(1, 10));
```

## for/in循环

```
var nums = [0, 1, 2, 3];
for(x in nums) {
  console.log(x);
}

var person = {name1: 'a', name2: 'b'};
for(x in person) {
  console.log(x + ": " + person[x]);
}
```

## for循环和for/in循环的区别

```
var nums = [];
nums[0] = 0;
nums[2] = 2;
nums[5] = 5;

// for循环没有跳过数组中的undefined元素
for(var i = 0; i < nums.length; i++) {
  console.log(i + ": " + nums[i]);
}

// for/in会跳过数组中的undefined元素
for(index in nums) {
  console.log(index + ": " + nums[index]);
}
```

## while循环

```
function sum(begin, end) {
  var rtn = 0;
  while(begin <= end) {
    rtn += begin;
    begin++;
  }
  return rtn;
}
```

## do/while循环

```
function sum(begin, end) {
  var rtn = 0;
  if(begin > end) return 0;
  do {
    rtn += begin;
    begin++;
  } while(begin <= end)
  return rtn;
}
console.log(sum(1, 10));
console.log(sum(10, 10));
console.log(sum(10, 9));
```

## break/continue

```
break用于跳出循环
continue用于跳出循环中的当前迭代，进入下一个迭代
```
