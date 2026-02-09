# Design Responsivo e Zoom

Esta seção descreve como utilizar unidades de medida flexíveis para garantir que a interface suporte um zoom de até 200% sem perda de conteúdo ou funcionalidade.

---

## Importância

* **Acessibilidade Visual:** Usuários com baixa visão frequentemente aumentam o zoom do navegador. Se o site usar apenas medidas fixas (px), o layout pode "quebrar" ou esconder textos.
* **Variedade de Dispositivos:** O uso de unidades relativas facilita a adaptação do layout para diferentes tamanhos de tela (monitores, tablets e smartphones).
* **Critério WCAG:** A conformidade com as normas WCAG exige que o conteúdo seja redimensionável sem a necessidade de tecnologias assistivas específicas.

---

## Como Implementar

A regra principal é **evitar o uso de `px` (pixels)** para tamanhos de fonte e larguras de recipientes, substituindo-os por unidades relativas.

### 1. Utilize `rem` e `em` para Fontes
* **`rem` (Root EM):** Baseia-se no tamanho da fonte padrão do navegador (geralmente 16px).
* **`em`:** Baseia-se no tamanho da fonte do elemento pai.

### 2. Layout Fluído
* **Unidades Flexíveis:** Use porcentagens (%) ou unidades de viewport (vw, vh) para containers.
* **Adaptação Dinâmica:** Garanta que o site "estique" ou "encolha" conforme o tamanho da tela do usuário.



### 3. Teste de Zoom de 200%
* **Rolagem Horizontal:** O critério de sucesso é que o site não deve gerar uma barra de rolagem horizontal em páginas de texto simples ao atingir 200% de zoom.
* **Preservação de Conteúdo:** Garanta que nenhum conteúdo ou funcionalidade seja cortado ou sobreposto durante o redimensionamento da página.

**Exemplo de CSS:**
```css
/* Errado: Tamanho fixo que não responde ao zoom do navegador */
p {
    font-size: 16px;
}

/* Correto: Se o usuário aumentar a fonte no navegador, o texto acompanha */
p {
    font-size: 1rem; /* Equivale a 16px por padrão */
}