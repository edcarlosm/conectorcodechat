<p align="center">
	<img src="https://github.com/code-chat-br/whatsapp-api/raw/main/public/images/code.png" alt="Quepasa-logo" width="500" />	
	<p align="center">Este código é uma implementação do Baileys , como um serviço RestFull Api, que controla as funções do whatsapp </p>
</p>
<hr />
<p align="left">
	<img src="https://whatsapp.com/favicon.ico" alt="WhatsAPP-logo" width="32" />
	<span>Grupo WhatsaAPP: </span>
	<a href="https://chat.whatsapp.com/CwcSUOcgPBL6lJWYyvA0NS
" target="_blank">Grupo</a>
</p>

----------------------------------------------------------------------------

</p>

**Gostou do Tutorial? Faça sua Contribuição**

<img src="https://github.com/EngajamentoFlow/quepasa/blob/main/Contribui%C3%A7%C3%A3o.png" alt="Quepasa-logo" width="200" />
</p>

**PIX CNPJ**

```
45959142000119	
```


----------------------------------------------------------------------------

----------------------------------------------------------------------------

</p>

**Instalando Integrador**

</p>
git clone https://github.com/w3nder/chatwoot-codechat
</p>
cd chatwoot-codechat
</p></p>
nano .env
</p>

 ```
PORT = 1234
CHATWOOT_ACCOUNT_ID = NUMEROCONTACHATWOOT
CHATWOOT_TOKEN = TOKENDOCHATWOOT
CHATWOOT_BASE_URL = URLDOCHATWOOT
CODECHAT_BASE_URL = URLCODECHAT
CODECHAT_API_KEY = TOKENCODECHAT
 ```
 
</p>
TOSIGN=true
</p>
npm install
</p>
npm run build
</p>
pm2 start dist/app.js --name NOMEQUEDESEJAR
</p>
sudo nano /etc/nginx/sites-available/conector
</p>

```
server {

  server_name conector.dominio.com.br;

  location / {

    proxy_pass http://127.0.0.1:1234;

    proxy_http_version 1.1;

    proxy_set_header Upgrade $http_upgrade;

    proxy_set_header Connection 'upgrade';

    proxy_set_header Host $host;

    proxy_set_header X-Real-IP $remote_addr;

    proxy_set_header X-Forwarded-Proto $scheme;

    proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;

    proxy_cache_bypass $http_upgrade;

    proxy_buffering off;

    proxy_cache off;

  }

  }
  
 ```

</p>
sudo ln -s /etc/nginx/sites-available/conector /etc/nginx/sites-enabled
</p>
sudo certbot --nginx
</p>
sudo service nginx restart
</p>


----------------------------------------------------------------------------

**Pronto tudo Funcionando**

----------------------------------------------------------------------------
----------------------------------------------------------------------------

</p>

**Gostou do Tutorial? Faça sua Contribuição**

<img src="https://github.com/EngajamentoFlow/quepasa/blob/main/Contribui%C3%A7%C3%A3o.png" alt="Quepasa-logo" width="200" />
</p>

**PIX CNPJ**

```
45959142000119	
```
----------------------------------------------------------------------------
