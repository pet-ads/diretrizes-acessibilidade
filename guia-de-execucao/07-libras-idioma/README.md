# Libras e Definição de Idioma

A acessibilidade linguística garante que o conteúdo seja compreendido por usuários que utilizam a Língua Brasileira de Sinais (Libras) como sua primeira língua ou que dependem de sintetizadores de voz para ler o texto escrito.

---

## 1. Definição do Idioma (Atributo lang)

Definir o idioma principal da página é o primeiro passo técnico para a acessibilidade. Isso permite que os leitores de tela utilizem a entonação, o sotaque e a pronúncia corretas ao processar o texto.

## 2. Acessibilidade em Libras
Para muitos usuários surdos, a Libras é a língua materna, e o português escrito pode ser uma segunda língua de difícil compreensão. Ferramentas de tradução digital ajudam a reduzir essa barreira.

### Implementação do VLibras
O **VLibras** é uma ferramenta gratuita que traduz conteúdos digitais (texto, áudio e vídeo) para Libras, tornando sites brasileiros muito mais acessíveis.

Para adicionar o tradutor ao seu site, você deve inserir o código oficial do widget logo após a abertura da tag `<body>`.

```html
<div vw class="enabled">
    <div vw-access-button class="active"></div>
    <div vw-plugin-wrapper>
        <div class="vw-plugin-top-wrapper"></div>
    </div>
</div>

<script src="[https://vlibras.gov.br/app/vlibras-plugin.js](https://vlibras.gov.br/app/vlibras-plugin.js)"></script>
<script>
    new window.VLibras.Widget('[https://vlibras.gov.br/app](https://vlibras.gov.br/app)');
</script>
```

## Dicas de Implementação Técnica

* **Posicionamento:** Por padrão, o ícone do **VLibras** fica fixado no lado direito da tela. Certifique-se de que ele não cubra elementos essenciais da interface, como botões de "Voltar", ícones de redes sociais ou janelas de chat de suporte.

* **Performance:** Como o script é carregado de um servidor externo (`gov.br`), a recomendação técnica de **ADS** é colocá-lo sempre no final do seu arquivo HTML, logo antes do fechamento da tag `</body>`. Isso garante que o carregamento visual do seu site não seja interrompido pelo plugin.

* **Visibilidade:** É uma boa prática informar aos usuários que o site possui suporte a Libras logo no início da página. Se você optar por utilizar uma imagem customizada para o acionador do widget, nunca esqueça de adicionar um atributo `alt` descritivo, como: `alt="Ícone de acessibilidade em Libras"`.

---

## Consulte a página oficial do Vlibras Widget
Para mais informações sobre customização e suporte técnico, acesse a documentação oficial:

* **[Acesse o VLibras Widget](https://vlibras.gov.br/doc/widget/installation/webpageintegration.html)**

