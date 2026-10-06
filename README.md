# SEI-GO — downloads

Assistente do SEI com inteligência artificial · Polícia Civil do Estado de Goiás · uso interno.

O SEI-GO é um painel no próprio computador que organiza a caixa do SEI, avisa quando chega processo, mostra a gestão
da unidade (produção, tempo parado, Acompanhamento Especial, prazos) e, se houver uma IA instalada, resume processos e
rascunha peças. **A IA nunca assina, tramita ou exclui nada no SEI.**

## Baixar a versão mais nova: 1.1.0

| Arquivo | Para quê | Tamanho |
|---|---|---|
| [**SEI-GO-Setup-1.1.0.exe**](https://github.com/windson83/sei-go-versoes/releases/download/v1.1.0/SEI-GO-Setup-1.1.0.exe) | Instalador (já traz o Python) | 35 MB |
| [SEI-GO-Manual-1.1.0.pdf](https://github.com/windson83/sei-go-versoes/releases/download/v1.1.0/SEI-GO-Manual-1.1.0.pdf) | Manual do usuário, passo a passo com telas | 5 MB |
| [SEI-GO-Manual-Tecnico-1.1.0.pdf](https://github.com/windson83/sei-go-versoes/releases/download/v1.1.0/SEI-GO-Manual-Tecnico-1.1.0.pdf) | Manual técnico, para a TI | 797 KB |

**Novidades da 1.1.0 — Textos prontos, blocos de assinatura, novos marcadores e iniciar processo**

- Textos prontos no Redigir (e em Mais ações → Responder com texto pronto): os Textos Padrão e os Favoritos da unidade no SEI. Veja o texto, use no editor (para ajustar ou pedir à IA) ou crie o documento direto com ele.
- Criar Texto Padrão novo pelo painel, inclusive a partir do texto que está no editor (Salvar como texto padrão).
- Blocos de assinatura: nova tela com os blocos recebidos e gerados, os documentos de cada bloco, quem já assinou e as anotações. Aviso no Windows quando chega bloco novo para a unidade. A assinatura continua no SEI.
- Criar marcador novo para a unidade, direto na janela do Marcador (nome, cor e descrição).
- Iniciar processo pelo painel: tipo (com busca entre todos), especificação, assuntos, interessados, observações e nível de acesso.
- Pela IA: consultar textos padrão, favoritos e blocos de assinatura, e criar documento já com um texto padrão ou favorito (sempre confirmado no painel).
- Documento restrito ou sigiloso: a hipótese legal agora é buscada no SEI quando a tela não a traz pronta.

Todas as versões: [página de versões](https://github.com/windson83/sei-go-versoes/releases).

## Como instalar

1. Baixe o **SEI-GO-Setup-1.1.0.exe** (link acima).
2. Dê dois cliques nele. Se o Windows avisar *"O Windows protegeu o computador"*, clique em **Mais informações** →
   **Executar assim mesmo**.
3. Clique em **Avançar** até o fim. Se o computador não tiver o Python, o instalador coloca sozinho
   (não precisa ser administrador). Leva de 2 a 6 minutos.
4. O painel abre no navegador. Siga o **Assistente de instalação**: escolha as IAs que você tem (ou nenhuma),
   digite **o seu** usuário e senha do SEI e escolha o órgão.
5. Pronto. O atalho **SEI-GO** fica no Menu Iniciar e na Área de Trabalho.

**Se o Windows bloquear o instalador** (computador com o *Controle Inteligente de Aplicativos* ligado), peça à
Divisão de Telecomunicações (DTEL) o pacote completo, que instala sem .exe.

## Como atualizar

**A partir da 0.9.4 o SEI-GO se atualiza sozinho**: confere uma vez por dia (e quando você entra no Windows),
baixa daqui, confere a assinatura digital e instala; o painel reinicia em 1 a 3 minutos e o Windows avisa.
Se preferir decidir a hora, desligue **Instalar atualizações sozinho** em Configuração: o painel mostra a faixa
**"Saiu o SEI-GO x.y.z"** com o botão **Atualizar agora**. Seu usuário, senha, cérebro local e histórico continuam.
Para conferir a qualquer hora: menu do seu nome → **Procurar atualização**.

Quem está numa versão anterior à 0.9.4 instala o **SEI-GO-Setup** novo uma vez, por cima; daí em diante é automático.
O arquivo `SEI-GO-atualizacao-x.y.z.bin` de cada versão é o pacote da atualização automática: não precisa baixá-lo.

## Segurança

- Baixe o SEI-GO **só desta página**.
- A senha do SEI é digitada no próprio painel e fica no cofre do Windows. Ninguém do suporte e nenhuma IA pede a sua senha.
- O SEI-GO só se atualiza sozinho com pacote baixado desta página **e assinado digitalmente** pelo SEI-GO; se a
  instalação falhar, ele volta para a versão anterior. Nunca pede senha para atualizar.
- Para conferir se o arquivo chegou íntegro, compare o hash SHA-256 com o `SHA256SUMS.txt` da versão
  (PowerShell: `Get-FileHash .\SEI-GO-Setup-1.1.0.exe -Algorithm SHA256`).

---

**Desenvolvimento e suporte:** Elder Windson Taveira Gonçalves — Chefe da Divisão de Telecomunicações · Delegacia-Geral – DGPC  
✉ elder.windson@pc.goias.gov.br · ☏ (62) 3201-2592 · policiacivil.go.gov.br
