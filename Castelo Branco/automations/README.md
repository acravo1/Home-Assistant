# ⚙️ Automations - Configurações de Automação

Automações simples e diretas implementadas em YAML.

## 📋 Automações Disponíveis

### 🚪 **Monitor de Portas**
**Ficheiro:** `portas_monitor.yaml`  
**ID:** `portas_monitor_geral`  
**Alias:** "Segurança: Monitor de Abertura de Portas"

**Descrição:** Monitora abertura de portas e envia avisos escalados através do script de escalamento.

**Sensores Monitorados:**
- Porta Principal (`binary_sensor.sensor_porta_principal`)
- Portão Garagem (`binary_sensor.sensor_portao_garagem`)

**Ações:**
- Ativa script `script.escalamento_aviso_porta`
- Identifica automaticamente a zona
- Passa o sensor como parâmetro

**Configuração:**
```yaml
trigger:
  - platform: state
    entity_id:
      - binary_sensor.sensor_porta_principal
      - binary_sensor.sensor_portao_garagem
    to: "on"

action:
  - action: script.escalamento_aviso_porta
    data:
      target_sensor: "{{ trigger.entity_id }}"
      nome_zona: >-
        {{ 'Porta Principal' if trigger.entity_id == 'binary_sensor.sensor_porta_principal' else 'Garagem' }}
```

---

## 🚀 Como Adicionar Novas Automações

1. Criar novo ficheiro YAML em `automations/`
2. Seguir estrutura padrão de automação Home Assistant
3. Documentar no README (este ficheiro)
4. Testar no Home Assistant

---

## 📝 Convenção de Nomenclatura

- **Ficheiros YAML:** `snake_case.yaml`
- **IDs de Automação:** `snake_case_com_prefixo`
- **Aliases:** Descrição clara em português

---

## 🔗 Links Úteis

- [Home Assistant Automations Docs](https://www.home-assistant.io/docs/automation/)
- [YAML Trigger Types](https://www.home-assistant.io/docs/automation/trigger/)

---

**Última atualização:** 2 de Setembro de 2026  
**Total de Automações:** 1 (Monitor de Portas)
