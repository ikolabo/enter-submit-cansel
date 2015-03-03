# inputが１つのフォームでEnterキーでSubmitされるのを防ぐ

```
$(document).ready(function(){

  // inputが１つのフォームで、Enter→submitを防ぐため。
  $("input:not(.allow_submit)").on("keypress", function(){
    return event.which !== 13;  // 13:Enter
  });

});
```
