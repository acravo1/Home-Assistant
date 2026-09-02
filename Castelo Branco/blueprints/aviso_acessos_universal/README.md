# 🚪 Aviso Acessos Universal - Blueprint

Sistema universal para notificações quando há acessos em portas, janelas ou outros sensores.

## 📋 Descrição

Este blueprint permite criar notificações automáticas e personalizadas sempre que um sensor de abertura muda de estado. Suporta múltiplos sensores, escalamento de avisos e integração com sistemas de notificação.

## 🎯 Funcionalidades

- ✅ Monitorização de múltiplos sensores
- ✅ Notificações customizáveis
- ✅ Escalamento de avisos por zona
- ✅ Filtros por hora/dia
- ✅ Histórico de eventos
- ✅ Integração com TTS

## 🛠️ Configuração

| Parâmetro | Tipo | Descrição |
|-----------|------|-----------|
| `target_sensor` | entity_id | Sensor a monitorizar (binary_sensor) |
| `zone_name` | texto | Nome descritivo da zona |
| `notification_service` | serviço | Serviço para enviar notificações |

## 📖 Documentação Completa

[👈 Voltar ao índice de blueprints](../README.md)

**Status:** 🔄 Em Desenvolvimento
