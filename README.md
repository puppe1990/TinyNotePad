# TinyNotePad
TinyNotePad build with HTML,CSS and Javascript.

Copy and paste on your browser:

data: text/html,<div style="position: fixed; text-align: right; top: 10px; right: 10px; text-transform: uppercase;">
<button onclick="download('file.txt','')">SAVE</button></div><div contenteditable style="width: 100%;height: 100%;" id="text">
</div><script>function download(filename, contentType){let content = document.getElementById("text").innerHTML;if(!contentType){
contentType = 'application/octet-stream';}var a = document.createElement('a');var blob = new Blob([content], {'type':contentType});a.href = window.URL.createObjectURL(blob);a.download = filename;a.click();}</script>
