# 🔋 Battery Alerts - Blueprint

Sistema automático de alertas e notificações para dispositivos com bateria fraca.

## 📋 Descrição

Este blueprint monitora os níveis de bateria de dispositivos e envia notificações automáticas quando a bateria cai abaixo de um limite configurável. Ideal para sensores wireless, telecomandos e dispositivos IoT.

## 🎯 Funcionalidades

- ✅ Monitorização automática de entidades com atributo `battery_level`
- ✅ Notificações personalizáveis por dispositivo
- ✅ Alertas em cascata (aviso, crítico, emergência)
- ✅ Integração com Alexa para avisos de voz
- ✅ Exclusão de horas de silêncio
- ✅ Histórico de notificações enviadas

## 🛠️ Configuração

| Parâmetro | Tipo | Descrição |
|-----------|------|-----------|
| `battery_sensor` | entity_id | Sensor de nível de bateria |
| `battery_threshold` | número | Percentagem mínima (padrão: 20%) |
| `notification_service` | serviço | Serviço para notificações |
| `alert_level` | select | Nível de alerta (baixo/médio/crítico) |

## 📖 Documentação Completa

[👈 Voltar ao índice de blueprints](../README.md)

**Status:** 🔄 Em Desenvolvimento