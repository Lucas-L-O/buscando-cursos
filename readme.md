**Alura Buscador de Cursos**
==========================

**Descrição**
---------------

Este é um projeto de busca de cursos desenvolvido em PHP, utilizando a biblioteca GuzzleHttp para realizar requisições HTTP e a biblioteca Symfony DomCrawler para extrair informações de HTML.

**Instalação**
---------------

Para instalar o projeto, você precisará ter o Composer instalado em sua máquina. Execute o seguinte comando:
```bash
composer install
```
**Uso**
-----

Para utilizar o buscador, você precisará criar uma instância da classe `Buscador` e passar uma URL para o método `buscar`. Por exemplo:
```php
$buscador = new Buscador(new GuzzleHttp\Client(), new Symfony\Component\DomCrawler\Crawler());
$cursos = $buscador->buscar('https://www.alura.com.br/cursos');
```
**Métodos**
------------

* `buscar(string $url)`: Realiza uma requisição GET para a URL fornecida e extrai os nomes dos cursos presentes na página.

**Requisitos**
--------------

* PHP 7.2 ou superior
* GuzzleHttp 6.3 ou superior
* Symfony DomCrawler 4.2 ou superior

**Contribuição**
--------------

Se você deseja contribuir com o projeto, por favor, faça um fork do repositório e envie um pull request com suas alterações.

**Licença**
------------

Este projeto é licenciado sob a licença MIT.

Espero que isso ajude! Se você precisar de mais informações ou quiser adicionar algo ao README, basta me informar.