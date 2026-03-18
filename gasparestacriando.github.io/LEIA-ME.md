# Arthur Gaspar — Portfolio
## Como usar esta pasta

### Estrutura
```
portfolio/
├── index.html          ← site completo (não editar o nome)
├── _redirects          ← necessário para o Cloudflare Pages
├── LEIA-ME.md          ← este arquivo
└── images/
    ├── wobble/         ← imagens do projeto Wobble x Make Some Noise
    ├── novinha/        ← imagens do projeto Novinha de Academia
    ├── barracao/       ← imagens do projeto Barracão Skateshop
    ├── dissidente/     ← imagens do projeto Dissidente Skate Video
    └── archive/        ← imagens do arquivo / recap
```

---

### Como adicionar suas imagens

1. Salve todas as imagens no formato **WebP** (melhor performance)
   - No Photoshop: Arquivo → Exportar → Exportar como → WebP
   - Tamanho recomendado: máximo 1800px de largura, qualidade 85%

2. Nomeie os arquivos de forma simples, sem espaços ou acentos:
   - ✅ `wobble-01.webp`, `barracao-logo.webp`
   - ❌ `Wobble 01.jpg`, `barracão-logo.png`

3. Coloque cada imagem na pasta do projeto correspondente

4. No `index.html`, substitua cada placeholder assim:

   **Antes:**
   ```html
   <div class="cs-gimg tall"><div class="ph pc1">01</div></div>
   ```
   **Depois:**
   ```html
   <div class="cs-gimg tall"><img src="images/wobble/wobble-01.webp" alt="Wobble poster 01"></div>
   ```

---

### Como publicar no Cloudflare Pages

1. Acesse **dash.cloudflare.com** e crie uma conta grátis
2. Vá em **Workers & Pages → Create application → Pages → Upload assets**
3. Dê o nome `arthur-gaspar` ao projeto
4. **Arraste a pasta `portfolio` inteira** para a área de upload
5. Clique em **Deploy site**
6. Site no ar em `arthur-gaspar.pages.dev`

### Para atualizar o site depois
- Volte em Workers & Pages → seu projeto → **Create new deployment**
- Arraste a pasta `portfolio` atualizada

---

### Domínio próprio (opcional)
- Compre em **registro.br** (~R$40/ano para .com.br)
- No Cloudflare Pages → Custom domains → Set up a custom domain
- Siga as instruções para apontar o DNS
