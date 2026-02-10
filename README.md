# diretrizes-acessibilidade-pet

Projeto destinado a padronizar a acessibilidade nos sistemas desenvolvidos pelo PET/ADS. Este guia detalha os elementos essenciais para garantir a inclusão e o cumprimento das normas WCAG.

## Seções de Execução

### 1. Texto Alternativo (Imagens)
Descreva todas as imagens para leitores de tela para garantir a compreensão do conteúdo visual.

[![SAIBA MAIS](https://img.shields.io/badge/SAIBA%20MAIS-007bff?style=for-the-badge)](./guia-de-execucao/01-texto-alternativo/)

### 2. Contraste de Cores
Aplicação do padrão WCAG AA com razão de 4.5:1 para garantir a legibilidade do texto.

[![SAIBA MAIS](https://img.shields.io/badge/SAIBA%20MAIS-007bff?style=for-the-badge)](./guia-de-execucao/02-contraste-cores/)

### 3. Design Responsivo e Zoom
Uso de unidades relativas (rem, em, %) para permitir zoom de até 200% sem quebrar o layout.

[![SAIBA MAIS](https://img.shields.io/badge/SAIBA%20MAIS-007bff?style=for-the-badge)](./guia-de-execucao/03-design-responsivo/)

### 4. HTML Semântico
Utilização de tags como `<header>`, `<nav>`, `<main>` e `<footer>` para navegação assistiva eficiente.

[![SAIBA MAIS](https://img.shields.io/badge/SAIBA%20MAIS-007bff?style=for-the-badge)](./guia-de-execucao/04-html-semantico/)

### 5. Links Descritivos e WAI-ARIA
Evite "Clique aqui" e utilize atributos ARIA para informar mudanças de estado em componentes dinâmicos.

[![SAIBA MAIS](https://img.shields.io/badge/SAIBA%20MAIS-007bff?style=for-the-badge)](./guia-de-execucao/05-links-e-aria/)

### 6. Formulários e Navegação
Manutenção de rótulos visíveis e suporte total à navegação por teclado (Tab).

[![SAIBA MAIS](https://img.shields.io/badge/SAIBA%20MAIS-007bff?style=for-the-badge)](./guia-de-execucao/06-navegacao-teclado/)

### 7. Libras e Definição de Idioma
Implementação do widget VLibras e configuração da tag `<html lang="pt-br">` para correta sintetização de voz.

[![SAIBA MAIS](https://img.shields.io/badge/SAIBA%20MAIS-007bff?style=for-the-badge)](./guia-de-execucao/07-libras-idioma/)

### 8. Lighthouse

Realização de auditorias automatizadas para identificar falhas de acessibilidade, validar o uso de textos alternativos e medir a conformidade do site com as diretrizes WCAG.

[![SAIBA MAIS](https://img.shields.io/badge/SAIBA%20MAIS-007bff?style=for-the-badge)](./guia-de-execucao/08-lighthouse/README.md/)