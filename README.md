# radar-nihon-videos

Hospedagem **temporária** dos vídeos curtos do Radar Nihon: o vídeo aprovado entra como anexo da release `fila`,
o TikTok puxa pela URL e o arquivo é **apagado logo depois da publicação**. Nada fica guardado aqui.

Script: `japan/automations/scripts/hospedar-video.sh` (repositório privado do projeto).

## GitHub Pages (desde 2026-11-09)

Os vídeos ficam em `v/` e são servidos em `https://andreyoshimura.github.io/radar-nihon-videos/v/<arquivo>.mp4`.
Esse prefixo é verificado no portal do TikTok (Manage URL properties) para a publicação por API, que só aceita
endereços verificados. O arquivo de verificação do TikTok fica na raiz e **não pode ser apagado**.
Depois de publicado, o vídeo é apagado de `v/` (o histórico do Git ainda guarda; repositório público, então só
vídeos que já seriam públicos).
