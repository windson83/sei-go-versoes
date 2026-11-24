# SEI-GO — downloads

Assistente do SEI com inteligência artificial · Polícia Civil do Estado de Goiás · uso interno.

O SEI-GO é um painel no próprio computador que organiza a caixa do SEI, avisa quando chega processo, mostra a gestão
da unidade (produção, tempo parado, Acompanhamento Especial, prazos) e, se houver uma IA instalada, resume processos e
rascunha peças. **A IA nunca assina, tramita ou exclui nada no SEI.**

## Baixar a versão mais nova: 1.9.1

| Arquivo | Para quê | Tamanho |
|---|---|---|
| [**SEI-GO-Setup-1.9.1.exe**](https://github.com/windson83/sei-go-versoes/releases/download/v1.9.1/SEI-GO-Setup-1.9.1.exe) | Instalador (já traz o Python) | 40 MB |
| [SEI-GO-Manual-1.9.1.pdf](https://github.com/windson83/sei-go-versoes/releases/download/v1.9.1/SEI-GO-Manual-1.9.1.pdf) | Manual do usuário, passo a passo com telas | 9 MB |
| [SEI-GO-Manual-Tecnico-1.9.1.pdf](https://github.com/windson83/sei-go-versoes/releases/download/v1.9.1/SEI-GO-Manual-Tecnico-1.9.1.pdf) | Manual técnico, para a TI | 1 MB |

**Novidades da 1.9.1 — Sua força: o brasão e o nome da sua instituição**

- Em Configuração → Sua força, escolha Polícia Civil, Secretaria de Segurança Pública, Polícia Penal, Polícia Militar ou Corpo de Bombeiros Militar, todas de Goiás.
- O brasão e o nome da força aparecem no alto do painel, no manual e nos relatórios em PDF. Polícia Civil e Polícia Penal já vêm com o brasão; nas outras aparece um emblema com a sigla até a imagem oficial ser carregada (PNG ou JPG).

Todas as versões: [página de versões](https://github.com/windson83/sei-go-versoes/releases).

## Como instalar

1. Baixe o **SEI-GO-Setup-1.9.1.exe** (link acima).
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
  (PowerShell: `Get-FileHash .\SEI-GO-Setup-1.9.1.exe -Algorithm SHA256`).

---

**Desenvolvimento e suporte:** Elder Windson Taveira Gonçalves — Chefe da Divisão de Telecomunicações · Delegacia-Geral – DGPC  
✉ elder.windson@pc.goias.gov.br · ☏ (62) 3201-2592 · policiacivil.go.gov.br
