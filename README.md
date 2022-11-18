## Documentasi
### Information
> Membuat bot Telegram gratis menggunakan <br/><b><a href="https://script.google.com/home/start?pli=1">Google Apps Script</a></b>

### Requirements 
buat bot terlebih dahulu <br/>
[BotFather](https://t.me/BotFather)

### Edit file
```core.gs```<br/>
```B_O_T__T_O_K_E_N``` Ganti dengan token bot kamu<br/>
```W_E_B__H_O_O_K``` Ganti dengan link hasil deploy<br/>
```ts
// identifikasi
const token = 'B_O_T__T_O_K_E_N';
const bot = new lumpia.init(token);

const userDB = new lumpia.userDB()
const button = lumpia.button
const markup = lumpia.markup
const helper = lumpia.helper
// handle komunikasi via POST dari Telegram ke (webhook) GAS
function doPost(e) {
  bot.doPost(e);}

bot.log_id = -1001234567890;
bot.options.prefix_command = '.!/';
bot.options.username = 'ScriptGooglebot';

function setWebHook() {
  let url = 'W_E_B__H_O_O_K';
  let result = bot.telegram.setWebhook(url);
  Logger.log(result);}

function cekUserProperties(){
  var r = userDB.getValues();
  Logger.log(r);}
```


link akses: 
<br/>{ Country } ganti nama folder yang tercantum di github MvBae
<br/>{ Jepang } ganti nama folder yang tercantum di github MvBae
<br/>{ Socho Shihatsu no Sappukei } ganti judul film yang tercantum di github MvBae
```ts
https://bayfrs.github.io/MvBae/{ Country }/{ Jepang }/{ Socho Shihatsu no Sappukei }.html
```

## Info
easy akses link film streaming and download
