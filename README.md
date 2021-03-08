## URL取得
```
URL取得ブックマークレット
javascript:(function(){
  var tmp = document.createElement('p');
  var pre = document.createElement('p');
  pre.style.userSelect = 'auto';
  tmp.appendChild(pre).textContent = location.href;
  document.body.appendChild(tmp);
  document.getSelection().selectAllChildren(tmp);
  document.execCommand('copy');
})();
```
## h2タイトル取得
```
javascript:(function(){
  var h2Array = document.getElementById('info').getElementsByTagName('h2')[0];
  var h2Title = h2Array.childNodes[1].textContent;
  var tmp = document.createElement('p');
  var pre = document.createElement('p');
  pre.style.userSelect = 'auto';
  tmp.appendChild(pre).textContent = h2Title;
  document.body.appendChild(tmp);
  document.getSelection().selectAllChildren(tmp);
  document.execCommand('copy');
})();
```
## h1タイトル取得ブックマークレット
```
javascript:(function(){
  var h1Array = document.getElementById('info').getElementsByTagName('h1')[0];
  var h1Title = h1Array.childNodes[1].textContent;
  var tmp = document.createElement('p');
  var pre = document.createElement('p');
  pre.style.userSelect = 'auto';
  tmp.appendChild(pre).textContent = h1Title;
  document.body.appendChild(tmp);
  document.getSelection().selectAllChildren(tmp);
  document.execCommand('copy');
})();
```
