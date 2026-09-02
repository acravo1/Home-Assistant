# 🏰 Castelo Branco - Home Assistant Automation Center

Central de automação inteligente e gestão para habitação em **Castelo Branco**, implementada com **Home Assistant**.

## 📋 Descrição Geral

Este módulo contém toda a configuração, automações avançadas, blueprints reutilizáveis e scripts personalizados para o sistema domotização de Castelo Branco. Inclui soluções para rega inteligente, segurança, notificações, monitorização de baterias e muito mais.

---

## 📁 Estrutura do Projeto

```
Castelo Branco/
├── README.md                          # Este ficheiro - Documentação principal
├── automations/                       # Automações da casa
│   └── portas_monitor.yaml            # Monitor de abertura de portas e garagem
├── blueprints/                        # Blueprints reutilizáveis para Home Assistant
│   ├── README.md                      # Lista completa de blueprints disponíveis
│   ├── aviso_acessos_universal/       # Blueprint para avisos de acessos
│   ├── battery_alerts/                # Blueprint para alertas de bateria baixa
│   ├── smart_dumb_dehumidifier/       # Blueprint para controlo inteligente de desumidificador
│   ├── smart_snailmail_box/           # Blueprint para caixa inteligente de correio
│   ├── smart_universal_calendar/      # Blueprint para calendário inteligente universal
│   └── watering_sector/               # Blueprint para rega otimizada por setores
├── scripts/                           # Scripts e rotinas personalizadas
│   ├── README.md                      # Lista de scripts disponíveis
│   ├── dynamic_notifications/         # Script de notificações dinâmicas com TTS
│   └── escalamento_aviso_porta/       # Script de escalamento de avisos de porta
├── views/                             # Visões do dashboard Lovelace
│   └── SistemaDeRega.yaml             # Dashboard de sistema de rega
└── manuais/                           # Documentação técnica e manuais
    ├── Manual_Nextcloud_Talk.md
    ├── Manual_Nextcloud_OnlyOffice.md
    ├── Manual_Paperless_NGX.md
    ├── Manual_Utilizacao_Familia.md
    ├── Plano_de_Emergencia_Familiar.md
    └── README.md                      # Índice de manuais
```

---

## 🚀 Funcionalidades Principais

### 🚪 Segurança & Monitorização
- **Monitor de Portas:** Detecção de abertura/fecho de portas principais e garagem
- **Escalamento de Avisos:** Sistema em cascata para avisos críticos

### 💧 Rega Inteligente
- **Rega Fracionada:** Sistema de 2 ciclos com pausa de absorção
- **Sensor de Humidade:** Controlo automático por nível de humidade
- **Interrupção Ativa:** Paragem imediata se desligado manualmente

### 🔋 Monitorização de Baterias
- **Alertas Dinâmicos:** Notificações quando bateria cai abaixo do limite
- **Integrações Alexa:** Avisos de voz prioritários

### 📢 Sistema de Notificações
- **TTS Dinâmicas:** Notificações de voz adaptadas a horários
- **Horários de Silêncio:** Respeita períodos configurados
- **Múltiplos Canais:** Suporta vários tipos de notificação

### 📅 Integrações Avançadas
- **Calendário Inteligente:** Eventos sincronizados
- **Nextcloud:** Suporte para Talk e OnlyOffice
- **Paperless-NGX:** Arquivo digital de documentos

---

## 📚 Componentes Disponíveis

### 🎨 Blueprints (7 disponíveis)
1. **Watering Sector** - Sistema de rega otimizado (⭐ Completo e documentado)
2. **Aviso Acessos Universal** - Notificações de acessos
3. **Battery Alerts** - Alertas de bateria
4. **Smart Dumb Dehumidifier** - Controlo de desumidificador
5. **Smart Snailmail Box** - Caixa inteligente de correio
6. **Smart Universal Calendar** - Calendário inteligente

Ver: [`blueprints/README.md`](./blueprints/README.md)

### 🔧 Scripts (2 principais)
1. **Dynamic Notifications** - Notificações TTS adaptadas
2. **Escalamento Aviso Porta** - Avisos em cascata para portas

Ver: [`scripts/README.md`](./scripts/README.md)

### 🎛️ Visões Dashboard
- **Sistema de Rega** - Dashboard completo de controlo de rega

Ver: [`views/`](./views/)

---

## 🛠️ Como Usar

### 1. Estrutura de Diretórios
Cada blueprint/script está organizado num diretório próprio com:
- Ficheiro YAML principal com a automação/blueprint
- `README.md` com documentação detalhada
- Ficheiros adicionais de suporte (se aplicável)

### 2. Importar um Blueprint
No Home Assistant:
1. Ir a: **Settings > Automations & Scenes > Blueprints > Import Blueprint**
2. Selecionar o ficheiro YAML do blueprint desejado
3. Preencher os parâmetros de entrada

### 3. Usar um Script
Referenciar no YAML de automações:
```yaml
action: script.[script_name]
data:
  param1: value1
  param2: value2
```

---

## 📖 Documentação Detalhada

| Componente | Documentação | Status |
|-----------|--------------|--------|
| Watering Sector | [📄 Detalhada](./blueprints/watering_sector/README.md) | ✅ Completa |
| Aviso Acessos | [📄 Início](./blueprints/aviso_acessos_universal/) | 🔄 Em desenvolvimento |
| Battery Alerts | [📄 Início](./blueprints/battery_alerts/) | 🔄 Em desenvolvimento |
| Smart Dehumidifier | [📄 Início](./blueprints/smart_dumb_dehumidifier/) | 🔄 Em desenvolvimento |
| Smart Snailmail | [📄 Início](./blueprints/smart_snailmail_box/) | 🔄 Em desenvolvimento |
| Smart Calendar | [📄 Início](./blueprints/smart_universal_calendar/) | 🔄 Em desenvolvimento |
| Dynamic Notifications | [📄 Início](./scripts/dynamic_notifications/) | 🔄 Em desenvolvimento |
| Escalamento Porta | [📄 Início](./scripts/escalamento_aviso_porta/) | 🔄 Em desenvolvimento |

---

## 🔒 Segurança

> ⚠️ **Nota Importante:** Nunca partilhe publicamente o seu ficheiro `secrets.yaml`, tokens de acesso ou senhas de rede no GitHub.

Consulte o `.gitignore` da raiz para ficheiros sensíveis excluídos.

---

## 🤝 Fluxo de Trabalho

### Estrutura Padrão para Novos Blueprints/Scripts:
1. Criar diretório em `blueprints/` ou `scripts/`
2. Adicionar ficheiro YAML com a automação
3. Criar `README.md` com:
   - Descrição breve
   - Funcionalidades
   - Configuração de inputs
   - Exemplos de uso
   - Troubleshooting

### Convenções de Nomenclatura:
- **Diretórios:** `snake_case` (ex: `watering_sector`)
- **Ficheiros YAML:** `snake_case` (ex: `watering_sector.yaml`)
- **READMEs:** `README.md` (SEMPRE MAIÚSCULA)

---

## 📞 Suporte & Troubleshooting

### Validação de Configuração
No Home Assistant:
**Developer Tools > YAML > Check Configuration**

### Visualizar Logs
```yaml
logger:
  default: info
  logs:
    homeassistant.components.automation: debug
```

---

## 📝 Changelog

### v1.0 (Setembro 2026)
- ✅ Estrutura base criada
- ✅ Watering Sector blueprint documentado
- 🔄 Restantes blueprints em desenvolvimento

---

## 📄 Documentação Adicional

Ver: [`manuais/`](./manuais/) para:
- Manual de Utilização para a Família
- Plano de Emergência Familiar
- Guias de Serviços (Nextcloud, Paperless, etc.)

---

**Última atualização:** 2 de Setembro de 2026  
**Versão Home Assistant:** Compatível com HA 2024.x+  
**Responsável:** @acravo1
