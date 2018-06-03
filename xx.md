	```js
  function User(name, password) {
    if(!(this instanceof User)){
      return new User(name, password);
    }
    this.name = name;
    this.password = password;
  }
  // 这种方式有缺点: 需要额外的函数调用,代价有点高.
  // 而且很难适用于可变参数,因为没有一种直接模拟apply方法
  // 将可变参数函数作为构造函数调用的方式
  ```