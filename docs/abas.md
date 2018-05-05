# Como criar uma estrutura de abas em um módulo

### 1 - Criando as Abas de Navegação
Cada item da lista será uma aba, siga as nomeclaturas dos IDs, e adicione os parametros corretos na função mostraNavegacaoAbas();

```html
<nav class="navegacaoAbas">

    <ul>
        <li id="aba1" onclick="mostraAba(1);">Geral</li>
        <li id="aba2" onclick="mostraAba(2);">Painel</li>
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
