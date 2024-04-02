# DiscordAutoLootboxes
Discord Auto Lootboxes (2024 April Fools)
# How to use
- Open Discord (prefer Discord web)
- Press Ctrl + Shift + I
- Paste bellow code in console tab.

```javascript
var thisToken=(webpackChunkdiscord_app.push([[""],{},e=>{for(let s in m=[],e.c)m.push(e.c[s])}]),m).find(e=>e?.exports?.default?.getToken!==void 0).exports.default.getToken();function sendRequest(){var e=new XMLHttpRequest;e.open("POST","https://discord.com/api/v9/users/@me/lootboxes/open",!0),e.setRequestHeader("Authorization",thisToken),e.setRequestHeader("X-Super-Properties","eyJvcyI6IldpbmRvd3MiLCJicm93c2VyIjoiQ2hyb21lIiwiZGV2aWNlIjoiIiwic3lzdGVtX2xvY2FsZSI6InZpIiwiYnJvd3Nlcl91c2VyX2FnZW50IjoiTW96aWxsYS81LjAgKFdpbmRvd3MgTlQgMTAuMDsgV2luNjQ7IHg2NCkgQXBwbGVXZWJLaXQvNTM3LjM2IChLSFRNTCwgbGlrZSBHZWNrbykgQ2hyb21lLzEyMy4wLjAuMCBTYWZhcmkvNTM3LjM2IiwiYnJvd3Nlcl92ZXJzaW9uIjoiMTIzLjAuMC4wIiwib3NfdmVyc2lvbiI6IjEwIiwicmVmZXJyZXIiOiIiLCJyZWZlcnJpbmdfZG9tYWluIjoiIiwicmVmZXJyZXJfY3VycmVudCI6IiIsInJlZmVycmluZ19kb21haW5fY3VycmVudCI6IiIsInJlbGVhc2VfY2hhbm5lbCI6InN0YWJsZSIsImNsaWVudF9idWlsZF9udW1iZXIiOjI4MDY4NiwiY2xpZW50X2V2ZW50X3NvdXJjZSI6bnVsbH0="),e.onload=function(){if(200==e.status)console.log(e.responseText);else if(429==e.status){var s=parseFloat(e.getResponseHeader("Retry-After"))||1;s=Math.round((s+.1)*10)/10,console.log("Too Many Requests. Retry after "+s+" sec(s)."),setTimeout(sendRequest,1e3*s)}else console.error(e.statusText)},e.onerror=function(){console.error("Request fail, try again...")},e.send()}sendRequest(),setInterval(sendRequest,2500);
```

- Done!

