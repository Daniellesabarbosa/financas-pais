# 📱 Guia — Finanças dos Pais no Celular

## O que você vai fazer
Publicar o app gratuitamente no **GitHub Pages** e instalar no seu
Android como se fosse um app de verdade (ícone na tela inicial,
abre em tela cheia, funciona offline).

---

## PARTE 1 — Criar conta no GitHub (se ainda não tiver)

1. Acesse **https://github.com**
2. Clique em **Sign up**
3. Informe e-mail, senha e um nome de usuário (ex: `joaosilva`)
4. Confirme o e-mail que vai chegar na sua caixa de entrada
5. Pronto — conta criada!

---

## PARTE 2 — Publicar os arquivos no GitHub Pages

### 2.1 Criar o repositório
1. Após entrar no GitHub, clique no botão verde **"New"** (ou no **+** no canto superior direito → *New repository*)
2. Em **Repository name**, digite exatamente: `financas-pais`
3. Deixe marcado como **Public**
4. Marque a opção **"Add a README file"**
5. Clique em **Create repository**

### 2.2 Subir os arquivos
1. Dentro do repositório recém-criado, clique em **"Add file"** → **"Upload files"**
2. Arraste **todos os arquivos** da pasta `financas-pwa` para a área indicada:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon-192.png`
   - `icon-512.png`
3. No campo **"Commit changes"** escreva: `Primeiro upload`
4. Clique em **Commit changes**

### 2.3 Ativar o GitHub Pages
1. No repositório, clique na aba **Settings** (engrenagem)
2. No menu lateral esquerdo, clique em **Pages**
3. Em **Source**, selecione **Deploy from a branch**
4. Em **Branch**, selecione **main** e a pasta **/ (root)**
5. Clique em **Save**
6. Aguarde cerca de **1-2 minutos**
7. A página vai mostrar o endereço do seu app, algo como:
   ```
   https://SEU-USUARIO.github.io/financas-pais
   ```
8. Guarde esse endereço — é o link do seu app!

---

## PARTE 3 — Instalar no celular Android

1. No celular Android, abra o **Chrome**
2. Acesse o endereço do seu app (ex: `https://SEU-USUARIO.github.io/financas-pais`)
3. Aguarde a página carregar completamente
4. O Chrome vai mostrar um banner na parte de baixo:
   **"Adicionar Finanças dos Pais à tela inicial"** → toque em **Adicionar**

   > Se o banner não aparecer automaticamente:
   > - Toque nos **três pontinhos** (⋮) no canto superior direito do Chrome
   > - Toque em **"Adicionar à tela inicial"**
   > - Confirme tocando em **Adicionar**

5. O ícone **"Finanças"** vai aparecer na sua tela inicial
6. Abra pelo ícone — vai abrir em tela cheia, sem barra do Chrome, como um app normal! ✅

---

## PARTE 4 — Atualizar o app no futuro

Quando Claude gerar uma versão nova do sistema:

1. Acesse seu repositório no GitHub
2. Clique no arquivo que quer atualizar (ex: `index.html`)
3. Clique no ícone de **lápis** (editar) no canto superior direito
4. Apague tudo e cole o novo conteúdo
5. Clique em **Commit changes**
6. Em 1-2 minutos o app já estará atualizado
7. No celular, abra o app e puxe para baixo para recarregar

---

## Perguntas frequentes

**Os dados ficam salvos se eu fechar o app?**
Sim! Os dados ficam no armazenamento interno do Chrome no seu celular. Funcionam offline também.

**Se eu desinstalar o app, perco os dados?**
Sim. Por isso use o botão **"Exportar"** dentro do app regularmente para fazer backup em um arquivo `.json`.

**Posso usar no celular de outra pessoa também?**
Sim, basta acessar o mesmo link e instalar. Mas os dados de cada celular são independentes.

**O app funciona sem internet?**
Sim! Após a primeira abertura, tudo fica em cache e funciona offline.

---

## Resumo dos arquivos

| Arquivo | Função |
|---|---|
| `index.html` | O sistema completo |
| `manifest.json` | Configurações do app (nome, ícone, cor) |
| `sw.js` | Service Worker — permite uso offline |
| `icon-192.png` | Ícone do app (tela inicial) |
| `icon-512.png` | Ícone do app (alta resolução) |
