# MS Nail Design — Landing Page

Página estática (HTML, CSS e JavaScript puros, sem build) com banner em vídeo, portfólio, serviços, como funciona e agendamento por WhatsApp.

## Estrutura

| Arquivo | Para que serve |
|---|---|
| `index.html` | Página principal |
| `privacidade.html` | Política de Privacidade |
| `hero.mp4` / `poster.jpg` | Vídeo do banner (sem áudio) e imagem de carregamento |
| `foto-1.jpg` … `foto-8.jpg` | Fotos do portfólio |
| `favicon.svg` | Ícone da aba do navegador |
| `vercel.json` | Configuração da Vercel (URLs limpas, cabeçalhos) |
| `robots.txt` | Permite a indexação pelos buscadores |

## Como editar

No topo do `<script>` do `index.html`, edite o bloco `CONFIG`:

- `whatsapp` e `mensagem`: número (com 55 + DDD) e texto de todos os botões "Agendar".
- `instagram`, `cidade`, `horarios` (opcionais): aparecem na chamada final se preenchidos.
- `videoPosition`: ponto focal do vídeo no computador e no celular.

Para trocar uma foto do portfólio, substitua o arquivo `foto-N.jpg` (de preferência com ~1000 px de largura).

## Publicar

1. Envie todos os arquivos para a **raiz** do repositório no GitHub.
2. Na Vercel: **Add New → Project**, escolha o repositório, **Framework Preset: Other**, sem comando de build, e clique em **Deploy**.
3. Cada novo commit no GitHub republica o site automaticamente.

## Observações

- As fontes vêm do Google Fonts; a página não usa cookies de rastreamento nem formulários.
- Se forem adicionadas estatísticas (ex.: Google Analytics), atualize `privacidade.html`.
