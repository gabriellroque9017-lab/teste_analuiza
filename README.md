# Portfólio — Ana Luiza Val

Site estático (HTML + JS puro), sem mensalidade, feito para o **GitHub Pages**.
Já vem com **20 fotos da Luh** e dois acessos: **visitante** (vê e entra em contato)
e **edição** (adiciona/remove fotos pelo próprio site).

---

## 1. Colocar no ar (uma vez só)

1. Crie um repositório no GitHub.
   - Para o endereço ficar `https://analuizaval.github.io`, chame o repositório de `analuizaval.github.io`.
   - Qualquer outro nome também funciona (fica `https://SEU-USUARIO.github.io/nome-do-repo`).
2. Suba **todos** os arquivos desta pasta, mantendo a estrutura:

   ```
   index.html
   fotos.json
   README.md
   assets/        (fundos: hero.jpg, sobre.jpg, contato.jpg)
   fotos/         (as 20 fotos: foto-01.jpg … foto-20.jpg)
   ```
3. Settings → Pages → Source: **Deploy from a branch**, branch `main`, pasta `/ (root)`. Salve.
4. Aguarde ~1 minuto e abra o endereço.

---

## 2. As fotos

A galeria já vem com **20 fotografias da Luh**, divididas em
**Ambientes, Gastronomia, Vinhos e Natureza**. Três delas também são os fundos
(capa = “Lampião”, sobre = “Fim de tarde”, contato = “Taças”).

### Adicionar / trocar — direto no site (sem programar)
O modo edição usa a **API do GitHub** para enviar fotos e atualizar o `fotos.json`.

**Criar o token (uma vez):**
1. GitHub → Settings → Developer settings → Personal access tokens → **Fine-grained tokens** → Generate new token.
2. Repository access → **Only select repositories** → marque este repositório.
3. Permissions → Repository permissions → **Contents: Read and write**.
4. Gere e **copie o token** (`github_pat_…`).

> O token é como a chave da casa: fica salvo **só no navegador dela**, nunca no site.

**Usar:**
1. Abra o site com `#estudio` no fim do endereço (ex.: `https://analuizaval.github.io/#estudio`) — ou clique em **“◦ estúdio”** no rodapé.
2. **Conectar** → preencha usuário, repositório e cole o token.
3. **Arraste as fotos** (ou “+ Adicionar fotos”). Sobem em **qualidade original**, sem recompressão.
4. Ajuste a **categoria**, reordene arrastando, exclua se quiser.
5. **Publicar alterações** → em ~1 min o portfólio atualiza para todos.

Quem não tem o token só vê o portfólio — não edita.

---

## 3. Editar textos (nome, frase, contato)

Tudo vive no `fotos.json` (dá para editar pelo lápis do GitHub):

- `titulo` — nome (marca, “Sobre” e rodapé). Já vem **Ana Luiza Val**.
- `eyebrow` — linha pequena acima do título da capa.
- `cidade` — cidade na capa.
- `categorias` — as abas de filtro.
- `contato.whatsapp` — só números. Já vem **5524993122505** (+55 24 99312-2505).
- `contato.instagram` — usuário, sem @ (já vem `analuizavalfotografia`).
- `contato.email` — e-mail (opcional).

Os textos maiores do “Sobre” ficam no `index.html` (seção `#sobre`).

---

## 4. Trocar os fundos (capa / sobre / contato)

São arquivos em `assets/`: `hero.jpg`, `sobre.jpg`, `contato.jpg`.
Para trocar, substitua o arquivo por outro de mesmo nome.

---

## 5. Fonte de exibição (Ogg Italic)

Os títulos usam a fonte **Ogg Italic** (paga, da Sharp Type). O arquivo dela **não** vai
incluso. Para ativá-la, coloque o arquivo em `assets/fonts/` com o nome
`Ogg-Italic.woff2` (e, se tiver, `Ogg-Italic.woff`). Enquanto o arquivo não estiver lá,
o site usa automaticamente a **Playfair Display Italic** (gratuita e parecida) como reserva.

## Notas
- **Qualidade:** miniatura na grade, tela cheia no clique — a partir do arquivo original.
  As fotos foram exportadas em ~1800px (grade leve e nítida); os originais completos da Luh
  podem ser subidos a qualquer momento pelo modo edição.
- **Domínio próprio** (ex.: `analuizaval.com`) é opcional e pago à parte; liga-se depois em Settings → Pages → Custom domain.
