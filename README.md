# sem
this will check the usn and current semeter 
<?xml version="1.0" encoding="utf-8"?>
<!DOCTYPE html PUBLIC "-//W3C//DTD/XHTML 1.1//EN"
"http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<title>lab prog 2b</title>
</head>
<body>
<script type="text/javascript">
function check()
{
var usn=document.getElementById('usn');
var sem=document.getElementById('sem');
var p1=/^[1-4][A-Z]{2}[0-9]{2}[A-Z]{2}[0-9]{3}$/;
var p2=/^[1-8]$/;

if(usn.value.match(p1)&&sem.value.match(p2))
    alert("value usn and semester");
else if(!usn.value.match(p1)&&!sem.value.match(p2))
    alert("both are invalid");
else if(!sem.value.match(p2))
   alert("invalid semester");
else
  alert("invalid usn");
}
</script>
usn<input type="text" id="usn">
sem<input type=text id="sem">
<input type="button" value="show" onclick="check()">
</body>
</html>
