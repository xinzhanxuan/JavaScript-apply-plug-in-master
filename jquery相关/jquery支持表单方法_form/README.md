# ajaxSubmit() 与 ajax() 的区别

## 语法区别:

```js
$("form").ajaxSubmit({
  type:"",
  url:"",
  data:{
    //可以增加额外参数(省略$("form").serialize()参数)  
  },
  success:function(info){
	//执行代码
  }
});

$.ajax({
  ...
  data : $("form").serialize(),
  ...
});
```



