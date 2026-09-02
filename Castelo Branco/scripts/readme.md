# 🔧 Scripts - Home Assistant

Coleção de scripts reutilizáveis para automações e rotinas personalizadas no Home Assistant.

## 📋 Scripts Disponíveis

### 1. 📢 **Dynamic Notifications** (Notificações Dinâmicas com TTS)
**Status:** 🔄 Em Desenvolvimento  
**Localização:** `./dynamic_notifications/`  
**Descrição:** Sistema de notificações dinâmicas com suporte a TTS (Text-to-Speech) e respeito pelos horários de silêncio configurados.

**Funcionalidades:**
- Notificações de voz (TTS) em português
- Respeita horários de silêncio
- Suporte a múltiplos canais
- Priorização de mensagens
- Integração com Alexa

**Ficheiro YAML:** `dynamic_notifications.yaml`

[📖 Ver Documentação](./dynamic_notifications/README.md)

---

### 2. 🚪 **Escalamento Aviso Porta** (Avisos em Cascata)
**Status:** 🔄 Em Desenvolvimento  
**Localização:** `./escalamento_aviso_porta/`  
**Descrição:** Script para escalamento automático de avisos quando há eventos em portas/janelas.

**Funcionalidades:**
- Escalamento em 3 níveis (suave → médio → crítico)
- Diferentes tipos de alerta por nível
- Respeita horários de silêncio
- Integração com notificações dinâmicas
- Histórico de eventos

**Ficheiro YAML:** `escalamento_aviso_porta.yaml`

[📖 Ver Documentação](./escalamento_aviso_porta/README.md)

---

## 🚀 Como Usar Scripts

### Chamar um Script de uma Automação

```yaml
automation:
  - trigger: ...
    action:
      - action: script.[script_name]
        data:
          param1: value1
          param2: value2
```

### Chamar um Script pelo Serviço

```yaml
service: script.[script_name]
data:
  param1: value1
  param2: value2
```

### Estrutura de um Script

Cada script está organizado assim:
```
[script_name]/
├── [script_name].yaml           # Ficheiro do script
└── README.md                    # Documentação detalhada
```

---

## 📝 Convenção de Nomenclatura

- **Diretórios:** `snake_case` (ex: `dynamic_notifications`)
- **Ficheiros YAML:** `snake_case` (ex: `dynamic_notifications.yaml`)
- **Documentação:** `README.md` (SEMPRE maiúscula)

---

## 🔗 Links Úteis

- [Home Assistant Scripts Docs](https://www.home-assistant.io/docs/scripts/)
- [Automations & Scripts](https://www.home-assistant.io/docs/automation/)

---

**Última atualização:** 2 de Setembro de 2026  
**Total de Scripts:** 2 (ambos em desenvolvimento)
