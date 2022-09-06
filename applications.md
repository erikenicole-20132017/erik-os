# Photo editor on Scratch 

https://scratch.mit.edu/projects/724178549/embed

# WarCat

https://scratch.mit.edu/projects/724533584/embed

# Kill the Fly

https://scratch.mit.edu/projects/724598911/embed

# Chick clicker 

https://scratch.mit.edu/projects/728388301/embed

# Calculator

```
<style>
* {
  margin:0;
  padding:0px;
  font-family: Segoe UI
}
#calc input {
  width:40px;
  height:40px;
  margin:1px;
  font-size:15px;
}
.area {
  margin-left: 4px;
  width:170px;
  height:30px;
  padding:2px;
  text-align:right;
  font-size:20px
}
</style>
<script>
function digit(n){
  if (document.form.res.value=='Y') {
    del();
  }
  document.form.monitor.value = document.form.monitor.value+n;
}

function ar(n){
  document.form.oper.value = n;
  document.form.last.value = document.form.monitor.value;
  document.form.monitor.value = '';
  document.form.res.value='';
}

function cancella() {
  var temp = document.form.monitor.value;
  document.form.monitor.value = temp.substring(0, temp.length-1);
}

function del() {
  document.form.monitor.value = '';
  document.form.last.value = '';
  document.form.oper.value = '';
  document.form.res.value = '';
}

function result() {
  if (document.form.res.value!='Y') {
  if (document.form.monitor.value && document.form.oper.value && document.form.last.value) {
    document.form.monitor.value = eval(document.form.last.value+document.form.oper.value+document.form.monitor.value);
    document.form.res.value='Y';
  }
  }
}

function perc() {
 if (document.form.res.value!='Y') {
  if (document.form.monitor.value && document.form.oper.value && document.form.last.value) {
    document.form.monitor.value = (document.form.last.value/100)*document.form.monitor.value;
    if (document.form.oper.value=='*' || document.form.oper.value=='/') {
      document.form.res.value='Y';
    }
  }
  }
}
</script>
<div id="calcolatrice">
  <form name="form">
    <input class="area" name="monitor" value="" placeholder="0">
    <input name="last" type="hidden" value="">
    <input name="oper" type="hidden" value="">
    <input name="res" type="hidden" value="">
    <table id="calc">
      <tr>
    <td><input type="button" value="C"  onclick="del();"></td>
    <td><input type="button" value="◄" onclick="cancella();"></td>
    <td><input type="button" value="%" onclick="perc();"></td>
    <td><input type="button" value="&divide;"  onclick="ar('/');"></td>
      </tr>   
      <tr>
    <td><input type="button" value="7" onclick="digit(7);"></td>
    <td><input type="button" value="8" onclick="digit(8);"></td>
    <td><input type="button" value="9" onclick="digit(9);"></td>
    <td><input type="button" value="*" onclick="ar('*');"></td>
      </tr>  
      <tr>
    <td><input type="button" value="4" onclick="digit(4);"></td>
    <td><input type="button" value="5" onclick="digit(5);"></td>
    <td><input type="button" value="6" onclick="digit(6);"></td>
    <td><input type="button" value="-" onclick="ar('-');"></td>
      </tr>  
      <tr>
    <td><input type="button" value="1" onclick="digit(1);"></td>
    <td><input type="button" value="2" onclick="digit(2);"></td>
    <td><input type="button" value="3" onclick="digit(3);"></td>
    <td><input type="button" value="+" onclick="ar('+');"></td>
      </tr>  
      <tr>
    <td><input type="button" value="0" onclick="digit(0);" ></td>
    <td><input type="button" value="00" onclick="digit('00');"></td>
    <td><input type="button" value=","onclick="digit('.');"></td>
    <td><input type="button" value="=" onclick="result();"></td>
      </tr>  
    </table>
  </form>
 </div>
```

Output: 
<div id="calcolatrice">
  <form name="form">
    <input class="area" name="monitor" value="" placeholder="0">
    <input name="last" type="hidden" value="">
    <input name="oper" type="hidden" value="">
    <input name="res" type="hidden" value="">
    <table id="calc">
      <tr>
    <td><input type="button" value="C"  onclick="del();"></td>
    <td><input type="button" value="◄" onclick="cancella();"></td>
    <td><input type="button" value="%" onclick="perc();"></td>
    <td><input type="button" value="&divide;"  onclick="ar('/');"></td>
      </tr>   
      <tr>
    <td><input type="button" value="7" onclick="digit(7);"></td>
    <td><input type="button" value="8" onclick="digit(8);"></td>
    <td><input type="button" value="9" onclick="digit(9);"></td>
    <td><input type="button" value="*" onclick="ar('*');"></td>
      </tr>  
      <tr>
    <td><input type="button" value="4" onclick="digit(4);"></td>
    <td><input type="button" value="5" onclick="digit(5);"></td>
    <td><input type="button" value="6" onclick="digit(6);"></td>
    <td><input type="button" value="-" onclick="ar('-');"></td>
      </tr>  
      <tr>
    <td><input type="button" value="1" onclick="digit(1);"></td>
    <td><input type="button" value="2" onclick="digit(2);"></td>
    <td><input type="button" value="3" onclick="digit(3);"></td>
    <td><input type="button" value="+" onclick="ar('+');"></td>
      </tr>  
      <tr>
    <td><input type="button" value="0" onclick="digit(0);" ></td>
    <td><input type="button" value="00" onclick="digit('00');"></td>
    <td><input type="button" value=","onclick="digit('.');"></td>
    <td><input type="button" value="=" onclick="result();"></td>
      </tr>  
    </table>
  </form>
 </div>

# Stopwatch
https://scratch.mit.edu/projects/728837766/embed
