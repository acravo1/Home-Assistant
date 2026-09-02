# 🎨 Blueprints - Home Assistant

Coleção de blueprints reutilizáveis para automações avançadas no Home Assistant.

## 📋 Blueprints Disponíveis

### 1. 🌊 **Watering Sector** (Rega por Setores)
**Status:** ✅ Completo e Documentado  
**Localização:** `./watering_sector/`  
**Descrição:** Sistema inteligente de rega com 2 ciclos, sensor de humidade, pausa de absorção e controlo de cooldown.

**Funcionalidades:**
- Rega fracionada com pausa intermédia
- Monitorização ativa de interrupção
- Salvaguarda periódica
- Notificações de voz (TTS)
- Tranca de cooldown nativa

[📖 Ver Documentação Completa](./watering_sector/README.md)

---

### 2. 🚪 **Aviso Acessos Universal** (Notificações de Acessos)
**Status:** 🔄 Em Desenvolvimento  
**Localização:** `./aviso_acessos_universal/`  
**Descrição:** Blueprint para avisos universais quando há acessos em portas/janelas.

**Ficheiro YAML:** `aviso_acessos_universal.yaml`

[📖 Ver Documentação](./aviso_acessos_universal/README.md)

---

### 3. 🔋 **Battery Alerts** (Alertas de Bateria)
**Status:** 🔄 Em Desenvolvimento  
**Localização:** `./battery_alerts/`  
**Descrição:** Sistema automático de alertas quando dispositivos têm bateria fraca.

**Ficheiro YAML:** `alerta_baterias_fracas_alexa.yaml`

[📖 Ver Documentação](./battery_alerts/README.md)

---

### 4. 💨 **Smart Dumb Dehumidifier** (Desumidificador Inteligente)
**Status:** 🔄 Em Desenvolvimento  
**Localização:** `./smart_dumb_dehumidifier/`  
**Descrição:** Controlo inteligente de desumidificadores com automações condicionais.

**Ficheiro YAML:** `gestao_desumidificador_inteligente.yaml`

[📖 Ver Documentação](./smart_dumb_dehumidifier/README.md)

---

### 5. 📮 **Smart Snailmail Box** (Caixa de Correio Inteligente)
**Status:** 🔄 Em Desenvolvimento  
**Localização:** `./smart_snailmail_box/`  
**Descrição:** Notificações inteligentes quando há correio na caixa.

**Ficheiro YAML:** `caixa_correio_inteligente.yaml`

[📖 Ver Documentação](./smart_snailmail_box/README.md)

---

### 6. 📅 **Smart Universal Calendar** (Calendário Universal Inteligente)
**Status:** 🔄 Em Desenvolvimento  
**Localização:** `./smart_universal_calendar/`  
**Descrição:** Integração de calendários com automações baseadas em eventos.

**Ficheiro YAML:** `calendario_inteligente_universal.yaml`

[📖 Ver Documentação](./smart_universal_calendar/README.md)

---

## 🚀 Como Usar Blueprints

### Importar um Blueprint no Home Assistant

1. **Menu:** Settings > Automations & Scenes > Blueprints
2. **Botão:** "Import Blueprint"
3. **Selecionar:** O ficheiro YAML do blueprint desejado
4. **Preencher:** Os parâmetros de entrada solicitados
5. **Confirmar:** Guardar a nova automação

### Estrutura de um Blueprint

Cada blueprint está organizado assim:
```
[blueprint_name]/
├── [blueprint_name].yaml        # Ficheiro do blueprint
└── README.md                    # Documentação detalhada
```

---

## 📝 Convenção de Nomenclatura

- **Diretórios:** `snake_case` (ex: `watering_sector`)
- **Ficheiros YAML:** `snake_case` (ex: `watering_sector.yaml`)
- **Documentação:** `README.md` (SEMPRE maiúscula)

---

## 🔗 Links Úteis

- [Home Assistant Blueprints Docs](https://www.home-assistant.io/docs/automation/blueprints/)
- [Blueprint Examples](https://github.com/home-assistant/blueprints)

---

**Última atualização:** 2 de Setembro de 2026  
**Total de Blueprints:** 6 (1 completo, 5 em desenvolvimento)
