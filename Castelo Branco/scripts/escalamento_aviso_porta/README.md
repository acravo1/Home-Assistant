# 🚪 Escalamento Aviso Porta - Script

Script para escalamento automático de avisos quando há eventos em portas/janelas.

## 📋 Descrição

Sistema em cascata para notificações de eventos de portas. Começa com avisos suaves e escala para alertas mais críticos se o evento não for resolvido.

## 🎯 Funcionalidades

- ✅ Escalamento em 3 níveis (suave → médio → crítico)
- ✅ Diferentes tipos de alerta por nível
- ✅ Respeita horários de silêncio
- ✅ Integração com script de notificações dinâmicas
- ✅ Histórico de eventos
- ✅ Confirmação de resolução

## 🔧 Parâmetros

| Parâmetro | Tipo | Descrição |
|-----------|------|-----------|
| `target_sensor` | entity_id | Sensor que disparou o evento |
| `zone_name` | texto | Nome da zona/local |
| `escalation_levels` | número | Quantos níveis de escalamento (1-3) |
| `timeout_per_level` | número | Tempo entre escalamentos (minutos) |

## 📖 Documentação Completa

[👈 Voltar ao índice de scripts](../README.md)

**Status:** 🔄 Em Desenvolvimento