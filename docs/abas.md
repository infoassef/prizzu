# Como criar uma estrutura de abas em um módulo0

### 1 - Criando as Abas de Navegação
Cada item da lista será uma aba, siga as nomeclaturas dos IDs, e adicione os parametros corretos na função mostraNavegacaoAbas();

```html
<nav class="navegacaoAbas">

    <ul>
        <li id="aba1" onclick="mostraAba(1);">Aba 1</li>
        <li id="aba2" onclick="mostraAba(2);">Aba 2</li>
    </ul>

</nav>
```

### 2 - Montando o conteúdo de uma aba
Dentro do próprio modo, você irá criar o conteúdo de cada aba como mostra o exemplo abaixo:

```html
<div id="conteudoAba1" class="conteudoAbas">
    <h2>Conteúdo da primeira aba</h2>
</div>

<div id="conteudoAba2" class="conteudoAbas">
    <h2>Conteúdo da segunda aba</h2>
</div>
```

### 3 - Validando um campo obrigatório via JS
Todas as abas são formadas por um mesmo form, com isso utilizam a mesma validação. Um campo ao ser validado será necessário fazer com que a aba que ele esteja seja exibida, desta forma:

<strong>Exemplo:</strong> 

<p>Nome do Campo     = <strong>campoTeste</strong></p>
<p>Localizado na Aba = <strong>2</strong></p>

```js

if(campoTeste == ""){
    swal('Atenção!', 'Informe o campo: Campo Teste!', 'error');
    setFocusSweetAlert('campoTeste');
    mostraAba(2);
    return false;
}

```
