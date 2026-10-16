# Máquina de Leads MXS

Prospecção de negócios locais que estão no Google Maps **sem site**, com prévia do site em PDF e abordagem pelo WhatsApp.

- `index.html` — a tela (arquivo único, Tailwind via CDN e JavaScript puro). A busca ainda é **simulada**.
- `whatsapp-local/` — WhatsApp local em Node (Baileys) que envia a mensagem e o PDF direto da tela, sem Docker e sem servidor.

## Como usar

1. Tenha o [Node.js](https://nodejs.org) 20 ou mais novo instalado.
2. Dê dois cliques em `whatsapp-local/iniciar.bat`. Na primeira vez ele instala as dependências; depois abre a tela e a janela do WhatsApp local, que mostra o **endereço** e a **API key**.
3. Na tela, clique em **Conectar WhatsApp**, cole a API key e leia o QR code com o celular (WhatsApp › Aparelhos conectados).
4. Busque, gere a **Prévia** e use **Enviar mensagem + PDF**.

Sem o WhatsApp local aberto, o botão abre o WhatsApp Web com a mensagem pronta.

## O que não vai para o GitHub

`whatsapp-local/sessao/` (login do WhatsApp), `whatsapp-local/config.json` (API key) e `node_modules/` estão no `.gitignore`. A API key é criada de novo em cada computador.
