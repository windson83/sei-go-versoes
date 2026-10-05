# SEI-GO — downloads

Assistente do SEI com inteligência artificial · Polícia Civil do Estado de Goiás · uso interno.

O SEI-GO é um painel no próprio computador que organiza a caixa do SEI, avisa quando chega processo, mostra a gestão
da unidade (produção, tempo parado, Acompanhamento Especial, prazos) e, se houver uma IA instalada, resume processos e
rascunha peças. **A IA nunca assina, tramita ou exclui nada no SEI.**

## Baixar a versão mais nova: 0.9.3

| Arquivo | Para quê | Tamanho |
|---|---|---|
| [**SEI-GO-Setup-0.9.3.exe**](https://github.com/windson83/sei-go-versoes/releases/download/v0.9.3/SEI-GO-Setup-0.9.3.exe) | Instalador (já traz o Python) | 33 MB |
| [SEI-GO-Manual-0.9.3.pdf](https://github.com/windson83/sei-go-versoes/releases/download/v0.9.3/SEI-GO-Manual-0.9.3.pdf) | Manual do usuário, passo a passo com telas | 3 MB |
| [SEI-GO-Manual-Tecnico-0.9.3.pdf](https://github.com/windson83/sei-go-versoes/releases/download/v0.9.3/SEI-GO-Manual-Tecnico-0.9.3.pdf) | Manual técnico, para a TI | 622 KB |

**Novidades da 0.9.3 — Aviso de versão nova mais claro**

- Botão Baixar destacado na faixa de versão nova.
- Janela de novidades com o botão Ir para o download.
- Manual do usuário com o capítulo Versão nova do SEI-GO.

Todas as versões: [página de versões](https://github.com/windson83/sei-go-versoes/releases).

## Como instalar

1. Baixe o **SEI-GO-Setup-0.9.3.exe** (link acima).
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

Quando sai uma versão nova, o painel mostra a faixa **"Saiu o SEI-GO x.y.z"** e o Windows avisa. Clique em
**Baixar**, baixe o novo **SEI-GO-Setup** e rode por cima. Seu usuário, senha, cérebro local e histórico continuam.
Para conferir a qualquer hora: menu do seu nome → **Procurar atualização**.

## Segurança

- Baixe o SEI-GO **só desta página**.
- A senha do SEI é digitada no próprio painel e fica no cofre do Windows. Ninguém do suporte e nenhuma IA pede a sua senha.
- O SEI-GO não baixa nem instala nada sozinho: o aviso de versão nova só traz você para esta página.
- Para conferir se o arquivo chegou íntegro, compare o hash SHA-256 com o `SHA256SUMS.txt` da versão
  (PowerShell: `Get-FileHash .\SEI-GO-Setup-0.9.3.exe -Algorithm SHA256`).

---

**Desenvolvimento e suporte:** Elder Windson Taveira Gonçalves — Chefe da Divisão de Telecomunicações · Delegacia-Geral – DGPC  
✉ elder.windson@pc.goias.gov.br · ☏ (62) 3201-2592 · policiacivil.go.gov.br
