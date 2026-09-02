# 📅 Smart Universal Calendar - Blueprint

Integração de calendários com automações inteligentes baseadas em eventos.

## 📋 Descrição

Blueprint para sincronizar eventos de calendários (Google, Nextcloud, CalDAV) com automações no Home Assistant. Permite acionar ações baseadas no começo/fim de eventos.

## 🎯 Funcionalidades

- ✅ Sincronização de múltiplos calendários
- ✅ Acionamento no começo de evento
- ✅ Acionamento no fim de evento
- ✅ Filtros por tipo de evento
- ✅ Notificações personalizadas
- ✅ Histórico de eventos processados

## 🛠️ Configuração

| Parâmetro | Tipo | Descrição |
|-----------|------|-----------|
| `calendar_entity` | entity_id | Entidade de calendário |
| `event_prefix` | texto | Prefixo para filtrar eventos (opcional) |
| `trigger_action` | select | Ação no começo/fim/ambos |
| `automation_on_start` | ação | Automação a correr no começo |
| `automation_on_end` | ação | Automação a correr no fim |

## 📖 Documentação Completa

[👈 Voltar ao índice de blueprints](../README.md)

**Status:** 🔄 Em Desenvolvimento
