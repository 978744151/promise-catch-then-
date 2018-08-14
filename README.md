

promise 2种catch不同的解决情况

// 例1  此种err ,err只能侦察到getdata() reject的异常情况。

```javascript
auto.getData().then(function(results){

    res.send(results)

},(err)=>{

    console.log('err')

})

```



​	// 例2  此种err ,catch  err能侦察到getdata()到后面.then的reject的异常情况。

```javascript
auot.getData().then(function(results){

    res.send(results)

}).catch(err=>{

    console.log('err')

})



```

![](C:\Users\Administrator\Desktop\ct\htmlcs\promise\img\微信图片_20180814143440.png)

