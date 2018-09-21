# 深入理解Java7 核心技术与最佳实践

java7 主要特性

#### 1. 在switch语句中可以使用字符串String类型.

#### 2. 支持在一个catch子句中同时捕获多个异常.

#### 3. try-with-resources语句,使它可以支持对资源进行管理，保证资源总是被正确释放.

#### 4. 优化变长参数的方法调用
```
public int sum(int... args){
    int result = 0;
    for(int value : args){
        result += value;
    }
    return result;
}
```

#### 5. 动态代理只支持对接口提供代理，一般的Java类不行.

#### 6. 增加了一个新的轻量级的任务执行框架, fork/join