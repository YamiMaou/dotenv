# YamiTec DotENV

# Instalação

para iniciar o projeto basta instalar apartir do composer  com o comando ```composer require yamitec/dot-env```

# Exemplo 

Para configurar o DotENV basta instanciar a classe ```\YamiTec\DotENV```.

o arquivo deve conter o seguinte conteúdo:

```
<?php
(new DotEnv(__DIR__ . '/.env'))->load();

echo getenv('APP_ENV');
// dev
echo getenv('DATABASE_DNS')

```
# ARQUIVO .ENV

E o seu arquivo de configuração deve seguir o exemplo:
```
[param]=[value]
APP_ENV=dev
DATABASE_HOST=127.0.0.1;
DATABASE_USER=username
DATABASE_PASSWORD=password

```

# Agradecimento

Equipe www.yamitec.com