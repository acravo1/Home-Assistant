# 💬 GUIA COMPLETO: CONFIGURAR E USAR O NEXTCLOUD TALK

O Talk é o nosso "WhatsApp" 100% privado. As mensagens, chamadas e videochamadas correm estritamente dentro do nosso Lenovo Host, livres de qualquer partilha de metadados com empresas externas.

---

## 📱 PASSO 1: INSTALAR E CONFIGURAR NO TELEMÓVEL

Para receber chamadas da família na rua, tem de configurar a aplicação no smartphone:

1. Vá à **Google Play Store** (Android) ou **App Store** (iPhone).
2. Pesquise por: `Nextcloud Talk` (instale a app oficial com o ícone azul de um balão de fala).
3. Abra a aplicação no telemóvel.
4. No primeiro campo, onde pede o **Endereço do Servidor**, digite a nossa rota externa segura:
   `https://duckdns.org`
5. Clique em **Avançar**.
6. O ecrã vai redirecioná-lo para o nosso portal de login. Insira o seu utilizador (`amc_manager` ou `fac_manager`) e password Google.
7. Clique em **Conceder Acesso**. A app está configurada e trancada!

---

## 💬 PASSO 2: INICIAR CONVERSAS E VIDEOCHAMADAS

### Como enviar uma mensagem:
1. Abra a app Talk no telemóvel ou aceda no computador via `http://talk.lenovo`.
2. Na listagem de conversas, clique no nome da pessoa com quem quer falar (Ana ou Francisco).
3. Digite a mensagem no fundo do ecrã e clique na seta de enviar. A mensagem cai no servidor local instantaneamente.

### Como fazer uma Videochamada Privada (WebRTC):
1. Entre na sala de chat da pessoa.
2. No canto superior direito, clique no ícone da **Câmara de Vídeo** ou do **Telefone**.
3. O telemóvel da outra pessoa vai começar a tocar imediatamente, mesmo que ela esteja na rua ligada aos dados móveis da NOS ou MEO.
4. **Resiliência Máxima:** Graças ao servidor de sinalização **STUN da Google** que cravámos no Kernel do Homelab, a ligação cruza as firewalls dos operadores e estabelece uma rota direta entre os smartphones com qualidade máxima de imagem e som.

---

## 🔒 PASSO 3: REINICIAR A APP EM CASO DE FALHA

Se notar que as mensagens não estão a atualizar ou as chamadas caem:
1. Feche completamente a aplicação no telemóvel (limpe-a da memória RAM das apps abertas).
2. Certifique-se de que tem internet ativa (Wi-Fi ou Dados Móveis).
3. Volte a abrir o Nextcloud Talk. O sistema faz um aperto de mão instantâneo com o Lenovo Host e descarrega todas as notificações pendentes.
