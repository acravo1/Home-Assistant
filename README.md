# Home Assistant Configuration & Automation

Repositório pessoal com as configurações, automações, guiões e integrações para o **Home Assistant**.

---

## 📋 Sobre o Projeto

Este repositório serve como ponto central de controlo, salvaguarda e documentação da minha instância do **Home Assistant**. Inclui ficheiros de configuração, integrações personalizadas, scripts de automação, definições para nós IoT (ex.: **ESPHome / ESP32 / Arduino**) e visões para os painéis de controlo (Lovelace).

---

## 🗂️ Estrutura do Repositório

```text
.
├── automations.yaml     # Regras de automação e gatilhos da casa
├── scripts.yaml         # Sequências de ações e rotinas personalizadas
├── scenes.yaml          # Cenas pré-configuradas (iluminação, ambientes)
├── configuration.yaml   # Configuração principal do Home Assistant
├── esphome/             # Ficheiros de configuração YAML para nós ESP32/ESP8266
├── custom_components/   # Componentes e integrações personalizadas (HACS)
└── README.md            # Documentação do repositório
```

---

## 🛠️ Tecnologias e Ecossistema

- **Core:** [Home Assistant](https://www.home-assistant.io/)
- **Microcontroladores:** ESP32, ESP8266 (através de [ESPHome](https://esphome.io/))
- **Protocolos & Comunicação:** MQTT, Zigbee, Wi-Fi, I2C, Modbus
- **Gestão de Componentes:** [HACS](https://hacs.xyz/) (Home Assistant Community Store)

---

## 🚀 Como Utilizar

1. **Clonar o Repositório:**
   ```bash
   git clone https://github.com/acravo1/Home-Assistant.git
   ```

2. **Ajustes de Segurança:**
   - Crie o seu próprio ficheiro `secrets.yaml` (não incluído por razões de segurança) para armazenar credenciais, chaves de API, palavras-passe e redes Wi-Fi.
   - Atualize as referências `!secret` no ficheiro `configuration.yaml`.

3. **Validar e Aplicar:**
   - Valide a configuração no Home Assistant (*Ferramentas do Desenvolvedor > YAML > Verificar Configuração*).
   - Recarregue ou reinicie a instância do Home Assistant.

---

## 🔒 Segurança

> ⚠️ **Nota Importante:** Nunca partilhe publicamente o seu ficheiro `secrets.yaml`, tokens de acesso ou senhas de rede no GitHub. Utilize o `.gitignore` para prevenir o envio inadvertido de dados sensíveis.

---

## 🤝 Contribuições e Feedback

Anotações, sugestões de melhoria nas automações ou otimizações no código YAML são sempre bem-vindas. Sinta-se à vontade para abrir uma *Issue* ou enviar um *Pull Request*.
README.md
A apresentar README.md