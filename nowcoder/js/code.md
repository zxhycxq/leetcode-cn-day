1、
var arr=[]; 
arr[0]=0; arr[1]=1; arr.foo='c'; 
console.log(arr.length)// 1.数组也是对象；2.对象不能用length返回其拥有的属性数量

2、
```js
function test(){
 var n=999;
 function add(){
 n++;
console.log(n);
}
return {n:n,add:add}
}

var result=test();
var result2=test();
result.add();
result.add();
console.log(result.n)
result2.add();
```

3、pow two
```js
var isPowerOfTwo = function(n) {
    if(n<0){return false}
    return n>0 && (n&(n-1))==0;
};
```
