# 💬 GUIA COMPLETO: CONFIGURAR E USAR O NEXTCLOUD TALK

O Talk é o nosso "WhatsApp" 100% privado. As mensagens, chamadas e videochamadas correm estritamente dentro do nosso Lenovo Host, livres de qualquer partilha de metadados com empresas externas.

---

## 📱 PASSO 1: INSTALAR E CONFIGURAR NO TELEMÓVEL

Para que a aplicação funcione e faça o aperto de mão com o nosso servidor, siga este roteiro de configuração:

### A) Se estiver FORA de casa (Na rua em 4G/5G):
1. Antes de abrir o Talk, abra a aplicação **WireGuard** no seu telemóvel.
2. Ative o botão do túnel **"CRAVO_HOMELAB_VPN"**. Isto estabelece uma ligação segura cifrada com o nosso servidor.

### B) Configuração da App Talk (Entrada Única):
1. Vá à **Google Play Store** (Android) ou **App Store** (iPhone).
2. Instale a app oficial **Nextcloud Talk** (ícone azul de um balão de fala).
3. Abra a aplicação no telemóvel.
4. No campo **Endereço do Servidor**, digite exatamente o nosso link local limpo e sem portas:
   `http://nextcloud.lenovo`
5. Clique em **Avançar**.
6. O ecrã vai abrir o nosso portal de login. Escolha **Entrar com o Google** e insira os seus dados de utilizador familiar (`amc_manager` ou `fac_manager`).
7. Clique no botão azul **Conceder Acesso**. A app faz a sincronização na RAM e está pronta a faturar no pico!

---

## 💬 PASSO 2: INICIAR CONVERSAS E VIDEOCHAMADAS

### Como enviar uma mensagem:
1. Abra a app Talk no telemóvel ou aceda no computador via `http://nextcloud.lenovo` clicando no ícone do balão de fala no topo.
2. Na listagem de conversas esquerda, clique no nome da pessoa (Ana ou Francisco).
3. Digite a mensagem no fundo do ecrã e envie.

### Como fazer uma Videochamada Privada (WebRTC):
1. Entre na sala de chat da pessoa.
2. No canto superior direito, clique no ícone da **Câmara de Vídeo**.
3. O telemóvel da outra pessoa vai tocar imediatamente. 
4. **Resiliência de Rede:** Graças ao servidor de sinalização **STUN da Google (stun.l.google.com:19302)** que configurámos no banco de dados do Nextcloud, os telemóveis descobrem as rotas de rede um do outro e mantêm a chamada estável e com qualidade máxima, sem timeouts de 5 segundos.
