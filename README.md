# Remotion — Boneco

Projeto Remotion em React + TypeScript.

## Configuração
- 1080 × 1920 (vertical)
- 30 fps
- Composições: `Boneco` e `Teste`

## Executar
```bash
npm install
npm run dev
```

No Remotion Studio, selecione a composição `Teste`.

## Renderizar a composição Teste
```bash
npm run render:teste
```

O vídeo será salvo em `out/teste.mp4`.

## Sincronizar o raio com a narração

Edite `QUADRO_DO_RAIO` no topo de `src/Root.tsx`. Em 30 fps, cada 30 quadros equivalem a 1 segundo (por exemplo, `120` = 4 segundos).

## Auditoria visual automática da composição Teste

Instale as dependências e execute:

```bash
npm install
npm run audit:teste
```

O script renderiza `Teste` em `out/auditoria/teste.mp4`, cria um PNG a cada 0,5 segundo (quadros 0, 15, 30, ... 285) e monta uma página de contato em `out/auditoria/index.html`. Abra essa página no navegador para inspecionar todos os prints.
