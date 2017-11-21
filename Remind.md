#Welcome to my Blog

##2017年11月21日
###js验证年月日(yyyy-mm-dd)格式

``` bash
    function dateCheck(dateString){
        var result = dateString.match(/^(\d{1,4})(-|\/)(\d{1,2})\2(\d{1,2})$/);
        if(result == null){
            return false;
        }
        var d = new Date(result[1],result[3]-1,$result[4])
        return d.getFullYear()==result[1]&&(d.getMonth()+1)==result[3]&&d.getDate()==result[4];
    }
```

###js验证年月日(yyyymm)格式
``` 
   function dateCheck(dateString) {
           var result = dateString.match(/^(\d{1,4})(\d{1,2})$/);
           if (result == null) {
               return false;
           }
           var d = new Date(result[1], result[2] - 1);
           return (d.getFullYear() == result[1] && (d.getMonth() + 1) == result[2]);
       }

```


