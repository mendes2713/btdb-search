# btdb-search
 A simple way to search for torrents in btdb.to

## BTDB-SEARCH
Html scraper of [BitTorrent Database](https://btdb.to/). Lets find a list of magnets links by query string. Return ArrayJson as result.

### Install

```
npm install btdb-search
```

### Search magnet links 
```javascript
var btdb = require('btdb-search');
btdb.search('Ubuntu').then(function (data) {
    console.log(data);
});
/*
 { magnet: 'magnet:?xt=urn:btih:8D2F56F13D1C52B866B26DE726716163A01D2BB6&dn=Lubuntu+12.10+from+LXDE+and+Ubuntu&tr=udp%3A%2F%2Ftracker.openbittorrent.com%3A80&tr=udp%3A%2F%2Fopen.demonii.com%3A1337&tr=udp%3A%2F%2Ftracker.coppersurfer.tk%3A6969&tr=udp%3A%2F%2Ftracker.opentrackr.org%3A1337%2Fannounce',
    name: 'Lubuntu 12.10 from LXDE and Ubuntu',
    size: '692.29 MB',
    popularity: '1099' },
  { magnet: 'magnet:?xt=urn:btih:51710E9E86907981A45C785575F56F650A2F793C&dn=ubuntu-14.04&tr=udp%3A%2F%2Ftracker.openbittorrent.com%3A80&tr=udp%3A%2F%2Fopen.demonii.com%3A1337&tr=udp%3A%2F%2Ftracker.coppersurfer.tk%3A6969&tr=udp%3A%2F%2Ftracker.opentrackr.org%3A1337%2Fannounce',
    name: 'ubuntu-14.04',
    size: '2.98 GB',
    popularity: '47' },
  { magnet: 'magnet:?xt=urn:btih:EB16DACA02F39EDA7A8EFDE6A4D849FA5EF1BDE5&dn=Ubuntu+12.04&tr=udp%3A%2F%2Ftracker.openbittorrent.com%3A80&tr=udp%3A%2F%2Fopen.demonii.com%3A1337&tr=udp%3A%2F%2Ftracker.coppersurfer.tk%3A6969&tr=udp%3A%2F%2Ftracker.opentrackr.org%3A1337%2Fannounce',
    name: 'Ubuntu 12.04',
    size: '2.69 GB',
    popularity: '3' },...
*/
