# Criando documentação com API Blueprint
Criando ciclo de vida de uma API com Blueprint + aglio + drakov + dredd 

# Instalar aglio
```
npm install -g aglio
```

# Gerar documentação
```
aglio -i api.apib --theme-full-width --no-theme-condense -o index.html
```

# Gerando um mock server
instalar mock server:
```
npm install -g drakov
```
Gerar o servidor:
```
drakov -f api.apib -p 4000
```

# Testando
instalar ferramenta apib2swagger:
```
npm install -g dredd
```
executar os testes:
```
dredd api.apib http://localhost:4000
```

# Author
@david_luk4s