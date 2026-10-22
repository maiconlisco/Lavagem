# App de Apontamento de Lavagem — Consórcio Nova Rota (Obra 60217)

App para o apropriador registrar, pelo celular, as lavagens do dia: fotos do caminhão sujo e limpo,
fotos da lubrificação, ficha de pneus, calibragem (SIM/NÃO), medidas dos pneus, horímetro e observação.
Funciona sem internet. No fim do dia, gera um arquivo (.json) que é importado no
"Relatorio de Lavagem - Nova Rota.html" para montar os relatórios diário, semanal e mensal.

## Arquivos (todos na mesma pasta)
- index.html: o app
- sw.js: guarda o app no celular para funcionar sem internet
- manifest.webmanifest, icon-192.png, icon-512.png: ícone e nome na tela inicial

## Atualizar o app
Se receber uma versão nova, é só substituir os arquivos no GitHub. O celular pega a versão nova
na próxima vez que abrir com internet (os apontamentos guardados não se perdem).

## Colocar no ar (uma vez só, grátis): GitHub Pages
1. Crie uma conta em github.com.
2. Clique em "New repository", dê o nome "lavagem", deixe "Public" e crie.
3. Clique em "uploading an existing file", arraste os 5 arquivos desta pasta e clique em "Commit changes".
4. Vá em Settings → Pages → em "Branch" escolha "main" e clique em Save.
5. Em 1 ou 2 minutos aparece o link, algo como: https://SEU-USUARIO.github.io/lavagem/

No GitHub fica só o app. As fotos e os apontamentos NUNCA vão para lá: ficam no celular
até o apropriador gerar o arquivo e mandar para você.

## No celular do apropriador (uma vez só)
1. Abra o link no Chrome (Android) ou Safari (iPhone), com internet.
2. Menu ⋮ → "Adicionar à tela inicial" / "Instalar app" (no iPhone: Compartilhar → "Adicionar à Tela de Início").
3. Pronto: o ícone "Lavagem" abre o app mesmo sem sinal.

Importante: não usar aba anônima e não "limpar dados do navegador", senão o histórico do celular é apagado.

## Uso diário
1. Abrir o app e conferir o dia e o nome.
2. "+ Equipamento" quando o caminhão chegar e "Tirar foto" no Sujo (a hora fica gravada).
3. Depois da lavagem: fotos do Limpo, da Lubrificação (e marcar os pontos), da ficha de pneus e
   calibragem SIM/NÃO. Pode alternar entre caminhões à vontade.
4. Pneus: tocar em cada posição e escolher marca, medida, condição (NOVO/REFORMADO), modelo e
   profundidade nas listas. Só o DOT é digitado. Se não achar na lista, escolher "Outro…" e digitar
   (o valor novo passa a aparecer na lista). Na próxima vez, o app já traz os pneus da última medição
   daquele caminhão: é só conferir e ajustar a profundidade.
5. No fim do dia: "Finalizar e enviar". O celular abre o compartilhar: mandar o arquivo por WhatsApp ou e-mail.

## No computador (controle de manutenção)
No "Relatorio de Lavagem - Nova Rota.html", passo 2, "Importar apontamento do celular (.json)".
Pode importar vários dias de uma vez. Eles ficam guardados no computador, então dá para gerar
o semanal e o mensal sem importar de novo.

Desenvolvido por Maicon Clóvis com apoio do Claude (Anthropic).
