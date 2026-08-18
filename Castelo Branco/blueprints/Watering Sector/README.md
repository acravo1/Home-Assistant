# 🌊 Automação de Rega Otimizada (Castelo Branco)

Blueprint avançado para controlo inteligente e fracionado de eletroválvulas de rega no ecossistema Home Assistant, desenhado com foco em eficiência hídrica e resiliência mecânica.

## 🚀 Funcionalidades Mestre

1. **Rega Fracionada em 2 Ciclos:** Divide o tempo total inserido no `input_number` em duas metades exatas, aplicando uma pausa intermédia (absorção) para evitar alagamentos e desperdício de água por escorrimento.
2. **Monitorização Ativa de Interrupção:** Utiliza um barramento `wait_for_trigger` em cada ciclo. Se desligares o interruptor físico ou virtual a meio da rega, o motor deteta o corte no milissegundo, cancela a automação e dispara um aviso de voz prioritário.
3. **Salvaguarda Periódica (Time Pattern):** Caso a quebra de humidade ocorra durante o período de resguardo, um gatilho secundário corre a cada 15 minutos para garantir que o setor não fica desidratado.
4. **Tranca de Cooldown Nativa:** Impede re-disparos sucessivos em loops curtos, lendo o tempo configurado em minutos e avaliando o atributo `last_triggered`.
5. **Notificações de Voz Inteligentes (TTS):** Integra-se com o script de mensagens dinâmicas, respeitando as restrições horárias de silêncio configuradas nos ajudantes da casa.

## 📂 Estrutura de Diretórios no Repositório

Para o Home Assistant indexar este Blueprint automaticamente via GitHub, o ficheiro deve residir estritamente neste caminho:
```text
homeassistant/
└── blueprints/
    └── automation/
        └── acravo1/
            └── Watering Sector/
                ├── Watering_Sector.yaml
                └── README.md
```

## 🛠️ Configuração dos Inputs

| Input ID | Tipo | Descrição |
|---|---|---|
| `sector_name` | Texto | Nome descritivo do setor (ex: Relvado Traseiras). |
| `soil_moisture_sensor` | Sensor | Entidade física do sensor de humidade do solo. |
| `moisture_limit` | input_number | Threshold/Limite mínimo de humidade que dispara a rega. |
| `watering_duration` | input_number | Tempo total de rega pretendido (em minutos). |
| `cooldown_duration` | input_number | Tempo de resguardo obrigatório entre regas (em minutos). |
| `watering_switch` | Switch | Relé/Eletroválvula física que controla a água. |
| `soak_duration_minutes` | Número | Tempo de descanso da terra entre o Ciclo 1 e o Ciclo 2. |
| `quiet_hours_start` | input_datetime | Início do horário de silêncio para avisos sonoros. |
| `quiet_hours_end` | input_datetime | Fim do horário de silêncio para avisos sonoros. |
