# Texto Alternativo (Imagens)

Esta seção detalha como implementar a descrição de imagens para garantir que o conteúdo visual seja acessível a todos os usuários.

---

## Importância

A inclusão de descrições acessíveis é fundamental por diversos motivos:

* **Leitores de Tela:** Permite que usuários cegos ou com baixa visão compreendam o que está sendo exibido na tela, já que o sintetizador de voz lerá o texto alternativo.
* **Problemas de Carregamento:** Caso a imagem não carregue devido a uma conexão lenta, o texto alternativo será exibido no lugar, mantendo o contexto da página.
* **SEO:** Motores de busca (como o Google) utilizam o atributo `alt` para indexar e entender o conteúdo das imagens.
* **Auditoria:** A ausência de descrições é um dos erros mais comuns que reduzem a nota de acessibilidade em ferramentas como o Lighthouse.

---

## Como Fazer

Para implementar corretamente, utilize o atributo `alt` dentro da tag `<img>` de HTML.

### Exemplo de Código:

```html
<img src="grafico-crescimento.png" alt="Gráfico de barras mostrando o crescimento de 20% nas vendas no primeiro semestre de 2025.">

<img src="grafico-crescimento.png"> <img src="grafico-crescimento.png" alt="imagem1"> ```

### Boas Práticas:
1. Seja Descritivo: Explique a função ou o conteúdo da imagem, não apenas "foto de um cachorro".
2. Imagens Decorativas: Se a imagem for apenas para enfeite (como uma linha divisória), use `alt=""` para que o leitor de tela a ignore.
3. Evite redundância: Não comece a descrição com "Imagem de..." ou "Foto de...", pois o leitor de tela já anuncia que se trata de uma imagem.

---
