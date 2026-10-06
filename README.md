# MONSTER — Arquivo de Investigação

Site interativo em português para explorar personagens, eventos, locais, temas e evidências de *MONSTER*. O acervo está no código do site; preferências como favoritos, histórico, progresso e modos de leitura são guardadas no navegador.

## Conteúdo do ZIP

- `src/` — código-fonte completo da interface e dos dados locais.
- `public/` — ícone e arquivos públicos.
- `dist/public/` — versão já compilada do site.
- `package.json`, `pnpm-lock.yaml` e configurações — dependências e execução independente deste arquivo, fora do workspace original.

## Executar o código-fonte

Requisitos: Node.js 20.19+ (ou 22.12+) e pnpm.

```bash
pnpm install
pnpm run dev
```

Abra o endereço local indicado pelo Vite (por padrão, `http://localhost:5173`). Para gerar uma nova versão compilada:

```bash
pnpm run build
pnpm run preview
```

O Vite usa `/` como caminho-base por padrão. `PORT` e `BASE_PATH` podem ser definidos para ajustar a porta e o caminho da publicação.

## Abrir a versão compilada

A pasta `dist/public/` contém a versão pronta. Sirva essa pasta por um servidor HTTP estático; por exemplo:

```bash
python3 -m http.server 8000 --directory dist/public
```

Depois abra `http://localhost:8000`. Não é necessário configurar API, banco de dados ou chaves para esta versão.
