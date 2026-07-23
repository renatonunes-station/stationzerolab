# Station Zero Lab — Landing Page

Landing page comercial estilo Apple, com hero em vídeo, lettering sincronizado, mockups animados por scroll e gradientes roxo/azul da marca.

## Estrutura
```
station-zero-site/
├── index.html          # o site (arquivo único, self-contained)
├── .nojekyll           # evita processamento Jekyll no GitHub Pages
└── assets/
    └── hero-journey.mp4 # (VOCÊ ADICIONA) vídeo do hero — baixe do chat do Cowork
```

> Sem o `assets/hero-journey.mp4`, o hero usa automaticamente um fundo em gradiente animado como fallback — o site continua funcionando.

---

## Publicar no GitHub Pages

### Opção A — Pelo site do GitHub (sem terminal, mais fácil)
1. Acesse https://github.com/new e crie um repositório novo, ex.: **`stationzerolab-site`** (público).
2. Na página do repositório vazio, clique em **“uploading an existing file”**.
3. Arraste **`index.html`**, **`.nojekyll`** e a pasta **`assets/`** (com o `hero-journey.mp4` dentro). Clique em **Commit changes**.
4. Vá em **Settings → Pages**.
5. Em **Build and deployment → Source**, escolha **Deploy from a branch**.
6. Em **Branch**, selecione **`main`** e a pasta **`/ (root)`**. Clique em **Save**.
7. Aguarde ~1 minuto. O site ficará em: `https://SEU-USUARIO.github.io/stationzerolab-site/`

### Opção B — Pelo terminal (git)
Requer git instalado e login no GitHub (via `gh auth login` ou token).

```bash
cd station-zero-site

# 1) crie o repositório no GitHub (site https://github.com/new) chamado stationzerolab-site
# 2) então:
git init
git add .
git commit -m "Station Zero Lab landing page"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/stationzerolab-site.git
git push -u origin main
```

Depois ative o Pages em **Settings → Pages → Deploy from a branch → main / root**.

---

## Domínio próprio (opcional)
Para usar `www.stationzerolab.com`, adicione um arquivo `CNAME` na raiz com o domínio e configure o DNS conforme a documentação do GitHub Pages.
