# 💨 Smart Dumb Dehumidifier - Blueprint

Sistema inteligente para controlo de desumidificadores com automações personalizadas.

## 📋 Descrição

Blueprint para automatizar desumidificadores "burros" (sem smart features nativas) através de relés inteligentes. Permite controlo baseado em humidade, temperatura e horários.

## 🎯 Funcionalidades

- ✅ Controlo automático por sensor de humidade
- ✅ Pausa automática por tempo ou humidade atingida
- ✅ Horários de operação personalizados
- ✅ Proteção contra sobreaquecimento
- ✅ Notificações de estado
- ✅ Histórico de operação

## 🛠️ Configuração

| Parâmetro | Tipo | Descrição |
|-----------|------|-----------|
| `dehumidifier_switch` | switch | Relé de controlo do desumidificador |
| `humidity_sensor` | entity_id | Sensor de humidade relativa |
| `humidity_threshold` | número | Humidade alvo (padrão: 60%) |
| `max_runtime` | número | Tempo máximo de funcionamento (minutos) |

## 📖 Documentação Completa

[👈 Voltar ao índice de blueprints](../README.md)

**Status:** 🔄 Em Desenvolvimento
