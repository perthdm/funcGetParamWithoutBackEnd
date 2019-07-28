# funcGetParamWithoutBackEnd

//Sent Param to another page with path url (Type : GET)
//Ex. www.9develop.com/?name=Eakkasit&age=21
//findGetParameter("age")  => return 21
//findGetParameter("name")  => return Eakkasit

<script>
function findGetParameter(parameterName) {
    var result = null,
        tmp = [];
    location.search.substr(1).split("&").forEach(function (item) {
          tmp = item.split("=");
          if (tmp[0] === parameterName){
            result = decodeURIComponent(tmp[1]);
          } 
    });
    return result;
}
console.log(findGetParameter("name"))
</script>

-----------------------------------------
comma for number Ex.300,000
.toLocaleString() 
-------------------------------------------
