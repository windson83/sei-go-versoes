# SEI-GO — downloads

Assistente do SEI com inteligência artificial · Polícia Civil do Estado de Goiás · uso interno.

O SEI-GO é um painel no próprio computador que organiza a caixa do SEI, avisa quando chega processo, mostra a gestão
da unidade (produção, tempo parado, Acompanhamento Especial, prazos) e, se houver uma IA instalada, resume processos e
rascunha peças. **A IA nunca assina, tramita ou exclui nada no SEI.**

## Baixar a versão mais nova: 1.4.0

| Arquivo | Para quê | Tamanho |
|---|---|---|
| [**SEI-GO-Setup-1.4.0.exe**](https://github.com/windson83/sei-go-versoes/releases/download/v1.4.0/SEI-GO-Setup-1.4.0.exe) | Instalador (já traz o Python) | 37 MB |
| [SEI-GO-Manual-1.4.0.pdf](https://github.com/windson83/sei-go-versoes/releases/download/v1.4.0/SEI-GO-Manual-1.4.0.pdf) | Manual do usuário, passo a passo com telas | 7 MB |
| [SEI-GO-Manual-Tecnico-1.4.0.pdf](https://github.com/windson83/sei-go-versoes/releases/download/v1.4.0/SEI-GO-Manual-Tecnico-1.4.0.pdf) | Manual técnico, para a TI | 1 MB |

**Novidades da 1.4.0 — Pastas de trabalho, fontes oficiais com citação e envio em lotes**

- Pastas de trabalho: aponte a pasta do contrato, do TR ou das normas da unidade; o SEI-GO converte para texto (o formato mais barato), indexa e usa na minuta e na análise, citando arquivo e página.
- Cada pasta tem tema, palavras-chave e processos ligados: entra sozinha nos processos certos ou você escolhe na hora de redigir. A pasta do computador nunca é alterada.
- Biblioteca de fontes oficiais: o Claude pesquisa na internet e o SEI-GO só baixa de site oficial (gov.br, leg.br, jus.br, mp.br, tc.br), guardando link e data de acesso. Fonte não oficial só entra com o seu aceite.
- Claude e Codex (MCP) ganham sei_pastas, sei_pasta_buscar, sei_pasta_ler e sei_fonte_oficial, com as skills sei-pastas-trabalho e sei-fontes-oficiais.
- Enviar processo em lotes (opcional): para mais de 10 unidades, como um grupo inteiro; uma confirmação, envio de 10 em 10 com progresso.
- Passo a passo para ligar o BitLocker no quadro de segurança e no manual.
- Segurança: a sessão do SEI nunca sai para outro site, e o texto gravado no SEI passa por limpeza (sem script, formulário ou imagem de fora), sem mudar a formatação.
- Correção: a mensagem de erro do quadro de segurança aparecia na janela de assinatura.

Todas as versões: [página de versões](https://github.com/windson83/sei-go-versoes/releases).

## Como instalar

1. Baixe o **SEI-GO-Setup-1.4.0.exe** (link acima).
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
  (PowerShell: `Get-FileHash .\SEI-GO-Setup-1.4.0.exe -Algorithm SHA256`).

---

**Desenvolvimento e suporte:** Elder Windson Taveira Gonçalves — Chefe da Divisão de Telecomunicações · Delegacia-Geral – DGPC  
✉ elder.windson@pc.goias.gov.br · ☏ (62) 3201-2592 · policiacivil.go.gov.br
