# Scanner de Códigos Pokémon TCG Live — Jutsu Geek

PWA gratuito para escanear QR codes dos cartões de código do Pokémon TCG Live e salvar automaticamente em uma planilha Google Sheets.

## Recursos

- Seleção das 20 coleções mais recentes (ou personalizada)
- Escaneamento rápido com câmera
- Confirmação visual (toast) após salvar
- Volta automaticamente para a câmera
- Lista dos últimos códigos da sessão
- 100% gratuito (PWA + Google Apps Script)

## Como configurar

### 1. Planilha Google

1. Crie uma nova planilha no Google Sheets
2. Na primeira linha coloque os cabeçalhos:

| Código | Coleção | Data/Hora | Status |

### 2. Apps Script

1. Na planilha, vá em **Extensões → Apps Script**
2. Apague o código padrão e cole o conteúdo do arquivo `apps-script.gs`
3. Salve (Ctrl+S)
4. Clique em **Implantar → Nova implantação**
5. Tipo: **Aplicativo da Web**
6. Executar como: **Eu**
7. Quem tem acesso: **Qualquer pessoa**
8. Clique em **Implantar**
9. Autorize as permissões quando pedir
10. Copie a **URL do aplicativo da Web**

### 3. Usar o scanner

1. Abra o arquivo `index.html` no navegador do celular (ou hospede em algum lugar gratuito como GitHub Pages)
2. Cole a URL do Apps Script no campo correspondente
3. Selecione a coleção
4. Clique em **Iniciar Câmera**
5. Aponte para o QR do cartão de código
6. O código é salvo automaticamente e a câmera continua pronta para o próximo

## Instalar como app (PWA)

No Chrome do Android:
1. Abra o scanner
2. Toque no menu (⋮)
3. **Adicionar à tela inicial**

## Fluxo de venda

1. Abra a planilha
2. Filtre ou copie os códigos desejados
3. Envie para o comprador
4. Apague a linha ou mude o Status para "Vendido"

## Notas

- O QR contém apenas o código alfanumérico (não a coleção). Por isso a coleção é selecionada antes do lote.
- A URL do Apps Script fica salva no navegador (localStorage).
- Funciona melhor no Chrome Android.

---
Feito para Jutsu Geek — Pau dos Ferros, RN