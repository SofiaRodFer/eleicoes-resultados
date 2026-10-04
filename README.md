# Voto a Voto · Eleições 2026

Painel estático em português para acompanhar a apuração oficial do TSE. Não precisa de Node, build ou servidor: a página consulta os arquivos públicos do TSE direto do navegador e atualiza a cada 15 segundos.

## Publicar no GitHub Pages

1. Envie `index.html`, `assets/br-map.svg` e este README para a branch `main`.
2. No repositório, abra **Settings → Pages**.
3. Em **Build and deployment**, selecione **Deploy from a branch**, branch `main` e pasta `/(root)`, e salve.
4. O GitHub mostrará o endereço público em **Settings → Pages**. Para este repositório, ele costuma ser `https://sofiarodfer.github.io/eleicoes-resultados/`.

## Dados e funcionamento

- Resultados: [API pública de divulgação do TSE](https://resultados.tse.jus.br/oficial/).
- Configuração das eleições e dos cargos carregada do TSE ao abrir a página.
- Consulta automática a cada 15 segundos. O painel só indica “Eleito segundo o TSE” quando esse estado aparece nos dados oficiais; liderança parcial é apresentada separadamente.
- O mapa é um SVG estático derivado da malha mínima das UFs fornecida pela [API de malhas do IBGE](https://servicodados.ibge.gov.br/api/v3/malhas/paises/BR?intrarregiao=UF&formato=application/vnd.geo+json&qualidade=minima).
- Site independente; não representa nem substitui o portal oficial do TSE.
