# Instruções de uso:

Primeiramente ao clonar o projeto, instale as dependências via composer:

```
composer install
```

Neste projeto estamos usando o PagSeguro no modelo checkout transparente, então será necessário que você adicione suas crendenciais no arquivo `.env`, através das seguintes chaves:

```
PAGSEGURO_ENV=sandbox
PAGSEGURO_EMAIL=
PAGSEGURO_TOKEN_SANDBOX=
PAGSEGURO_CHARSET=UTF-8
```

Estas chaves podem ser obtidas através de sua conta no PagSeguro Sandbox: **[sandbox.pagseguro.uol.com.br](http://sandbox.pagseguro.uol.com.br)**.

Estamos usando o gerenciamento de assets via Laravel Mix, para isso instale as dependências com o npm ou yarn:

```
npm install
```
E depois execute o:

```
npm run dev
```

para gerar o build frontend de desenvolvimento.

Se você receber o erro de key não existente em seu browser, não esqueça de rodar o:

```
php artisan key:generate
```
na raiz do projeto. Aliás todos os comandos são executados na raiz do projeto.

Por fim, crie sua base de escolha e informe os dados de acesso no arquivo `.env` e execute as migrações do projeto:

```
php artisan migrate
```

E em seguida já execute seu built-in server:

```
php artisan serve
```

Bons estudos!