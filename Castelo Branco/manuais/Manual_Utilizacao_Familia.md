# 📖 GUIA DE ACESSO AO COCKPIT DIGITAL DA FAMÍLIA (CRAVO HOMELAB)

Este é o documento unificado e soberano para a utilização das plataformas digitais instaladas no nosso servidor central. Todos os serviços correm de forma privada dentro das nossas quatro paredes, livres de publicidade ou espionagem exterior.

---

## 📡 1. REGRAS DE REDE (COMO ACEDER EM CASA)

Para simplificar a utilização, eliminámos os números de portas complexos. Sempre que estiver ligado ao Wi-Fi de casa, pode aceder a qualquer plataforma digitando estes nomes limpos diretamente na barra de endereços do browser (Chrome, Safari ou Edge):

*   **Ficheiros e Nuvem da Família:** http://nextcloud.lenovo
*   **Arquivo de Documentos e Faturas:** http://paperless.lenovo
*   **Chat e Videochamadas Privadas:** http://talk.lenovo
*   **Painel de Controlo da Casa:** https://homeassistant.lenovo

---

## 📑 2. NEXTCLOUD (OS NOSSOS FICHEIROS E DOCUMENTOS)

A nossa nuvem substitui na totalidade o Google Drive e o Dropbox. Aqui salvaguardamos fotografias, cópias de segurança e ficheiros importantes.

### 👥 Contas Autorizadas:
*   **Ana:** Nome de utilizador: amc_manager
*   **Francisco:** Nome de utilizador: fac_manager
*   *Nota: O acesso está blindado e unificado através do Social Login da Google via Authentik SSO.*

### 🛠️ O Editor de Documentos (ONLYOFFICE Integrado):
Ao abrir qualquer documento de texto ou folha de cálculo dentro do Nextcloud, o editor **ONLYOFFICE** carrega de forma nativa e automática. Não necessita de instalar o Microsoft Office no computador. As alterações são guardadas instantaneamente no SSD do servidor.

---

## 🗃️ 3. PAPERLESS-NGX (O COFRE DE FATURAS DIGITALIZADAS)

O nosso arquivo morto digital já conta com **12.574 documentos e faturas** processados sem qualquer duplicação. 

### 🚀 Como utilizar no dia a dia:
1.  Aceda a http://paperless.lenovo
2.  Faça o login com as suas credenciais seguras.
3.  **A Pesquisa Inteligente:** Pode pesquisar por qualquer palavra (ex: "Continente", "Seguro", "Rega", "Fatura"). O motor interno lê o texto de dentro dos PDFs digitalizados e encontra o documento em menos de 1 segundo.
4.  **Organização Eficiente:** O sistema aplica etiquetas automáticas baseadas em inteligência artificial para separar as despesas por categorias.

---

## 💬 4. NEXTCLOUD TALK (O NOSSO WHATSAPP PRIVADO)

Para garantir que as nossas conversas e videochamadas familiares não são lidas por empresas externas, o Nextcloud Talk gere as comunicações de forma totalmente cifrada e ponto-a-ponto (WebRTC).

### 📱 Configuração no Telemóvel:
1.  Instale a aplicação gratuita **Nextcloud Talk** a partir da Google Play Store ou Apple App Store.
2.  No campo do endereço do servidor, digite a nossa rota externa segura: https://duckdns.org
3.  Insira o seu utilizador familiar (amc_manager ou fac_manager).

### 🎥 Chamadas Resilientes:
Configurámos os servidores de sinalização **STUN da Google (porto 19302)** em background. Isto garante que, mesmo que esteja na rua ligado à rede móvel 4G/5G da NOS ou da MEO, a chamada toca instantaneamente em casa com qualidade máxima e sem quebras de ligação.

---

## 🚨 5. SEGURANÇA E SUPORTE DE REFORMA

Se algum serviço apresentar lentidão, o cockpit de monitorização central (**Uptime Kuma**) valida o estado de saúde do hardware de 60 em 60 segundos na porta de operações. O sistema de alarme físico está permanentemente interligado em background, mantendo o cartão SIM ativo como canal redundante de chamadas de emergência direta para os telemóveis.
