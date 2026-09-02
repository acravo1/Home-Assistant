# 📮 Smart Snailmail Box - Blueprint

Sistema inteligente para notificações quando há correio na caixa de correio.

## 📋 Descrição

Blueprint que monitora um sensor de movimento/abertura na caixa de correio e envia notificações quando há novo correio. Ideal para não perder nenhuma encomenda ou carta importante.

## 🎯 Funcionalidades

- ✅ Detecção de movimento/abertura
- ✅ Notificações imediatas de novo correio
- ✅ Confirmação de recolha
- ✅ Histórico de eventos
- ✅ Filtro de falsos positivos
- ✅ Integração com Alexa

## 🛠️ Configuração

| Parâmetro | Tipo | Descrição |
|-----------|------|-----------|
| `motion_sensor` | entity_id | Sensor de movimento/abertura |
| `notification_service` | serviço | Serviço para notificações |
| `debounce_time` | número | Tempo de proteção contra tremulações (segundos) |
| `quiet_hours_start` | time | Início do silêncio |
| `quiet_hours_end` | time | Fim do silêncio |

## 📖 Documentação Completa

[👈 Voltar ao índice de blueprints](../README.md)

**Status:** 🔄 Em Desenvolvimento
