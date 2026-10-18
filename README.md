# Estradinhas RS 🗺️🚗

Aplicativo web para passeios de carro em estradas vicinais, começando na região de Tapejara/RS.

## Abrir
Quando o GitHub Pages estiver ativado:
https://iurifinger.github.io/Estradinha/

## Como começar
1. Abra o site no Chrome Android (requer HTTPS para GPS) e use o menu para adicionar à tela inicial.
2. Defina a base tocando no mapa ou usando **Minha localização**.
3. Carregue as estradas reais do OpenStreetMap e escolha o raio.
4. Escolha um limite de quilômetros, gere um circuito e confira os trechos sugeridos.
5. Abra cada etapa no Google Maps para navegar (a rota pode ser recalculada pelo Google).
6. Use **Explorar** para registrar o GPS, com o aplicativo em primeiro plano. Finalize o passeio.
7. Faça backup do histórico no painel **Histórico**.

## Limitações importantes
- **Protótipo V1**, não navegação automotiva certificada: algumas estradas podem ser privadas, interrompidas ou intransitáveis.
- O OpenStreetMap pode não conter todas as vias ou ter informações desatualizadas.
- Carregar estradas usa a API pública Overpass e internet; ela pode demorar ou falhar.
- Abrir o Google Maps em primeiro plano pode interromper o rastreamento GPS neste aplicativo web. Para rastrear em segundo plano de forma confiável, será necessário um aplicativo Android dedicado.
- Os pontos de GPS são associados aproximadamente a trechos de 100 m; erros de precisão podem marcar um trecho incorreto.
- O progresso fica no armazenamento local do navegador; não há conta ou sincronização. Use **Exportar backup** frequentemente e antes de limpar dados do navegador.
- Quando o mapa está carregando, a localização-base é enviada ao serviço público Overpass; ao abrir navegação, os pontos da rota são enviados ao Google Maps.
- O modo offline pode conservar a interface após o primeiro acesso, mas não substitui mapas offline.

## Arquivos
`index.html` contém a interface e a lógica.
`manifest.webmanifest` e `service-worker.js` dão suporte à instalação web.
`icon.svg` é o ícone.

## Publicação no GitHub Pages
Em **Settings → Pages → Build and deployment** selecione **Deploy from a branch**, ramo **main**, pasta **/(root)** e clique em **Save**. O site pode demorar alguns minutos a ficar disponível.

Projeto separado de OperVision.