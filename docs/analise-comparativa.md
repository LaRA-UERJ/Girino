# Análise Comparativa — Girino vs Trabalhos Relacionados

Review sistemático dos trabalhos mais próximos do Girino, com análise de lacunas e diferenciais.

---

## 1. Análise dos Trabalhos Mais Próximos

### 1.1 Mini bancada de baixo custo com motores CC e encoder (Cabral et al., 2025)

**Veículo:** Ciência e Natura (UFSM), Vol. 47, No. esp. 4
**DOI:** https://doi.org/10.5902/2179460X92211

**Descrição:** Bancada didática de baixo custo com motor DC e encoder para ensino de controle realimentado em engenharia. Inclui modelagem matemática do motor, derivação da função de transferência e projeto de controlador digital discreto para controle de velocidade angular. Validação via MATLAB/Simulink.

| Aspecto | Cabral et al. (2025) | Girino |
|---|---|---|
| Microcontrolador | Arduino | ESP8266 WROOM |
| Motor | DC com encoder | DC com encoder (LPD3806-600BM) |
| Encoder | Sim | Sim (600 PPR) |
| PID | Sim (discreto) | Planejado |
| Interface | MATLAB/Simulink | **Web embarcada (navegador)** |
| Wi-Fi | Não | **Sim** |
| OTA | Não | **Sim (ElegantOTA)** |
| Modelagem matemática | **Sim (completa)** | A fazer |
| Custo | Baixo | Baixo |
| Open-source | Parcial | **Sim (tripla licença)** |

**Pontos fortes:** Modelagem matemática rigorosa, validação MATLAB/Simulink, aplicação em engenharia.
**Lacunas:** Sem conectividade, depende de MATLAB (software proprietário e caro), sem OTA.

---

### 1.2 Análise do controle PID aplicado no controle de velocidade de um motor CC (Alexandre et al., 2025)

**Veículo:** Revista de Engenharia e Tecnologia (UEPG), Vol. 17, No. 1
**URL:** https://revistas.uepg.br/index.php/ret/article/view/24725

**Descrição:** Controle PID de velocidade de motor DC usando Arduino UNO R3, encoder rotativo e ponte H L298N. Sintonia via método Cohen-Coon. Aplicação SCADA para monitoramento. Testes em 200, 275 e 120 RPM com erro em regime permanente próximo de zero.

| Aspecto | Alexandre et al. (2025) | Girino |
|---|---|---|
| Microcontrolador | Arduino UNO R3 | ESP8266 WROOM |
| Motor | DC | DC |
| Encoder | Rotativo | LPD3806-600BM |
| Driver | L298N (ponte H) | MOSFET genérico |
| PID | Sim (Cohen-Coon) | Planejado |
| Interface | SCADA desktop | **Web embarcada** |
| Wi-Fi | Não | **Sim** |
| OTA | Não | **Sim** |
| Monitoramento | Aplicativo dedicado | **Navegador web** |
| Sintonia | Cohen-Coon | A definir |

**Pontos fortes:** Hardware quase idêntico ao Girino, resultados experimentais validados, método de sintonia definido.
**Lacunas:** Sem Wi-Fi, sem web, sem OTA, aplicativo SCADA requer instalação.

---

### 1.3 Bancada Didática para Controle de Velocidade de Motor CC (Segundo et al., 2019)

**Veículo:** SBAI — Simpósio Brasileiro de Automação Inteligente
**URL:** https://proceedings.science/sbai-2019/trabalhos/desenvolvimento-de-uma-bancada-didatica-para-praticas-de-controle-de-velocidade

**Descrição:** Bancada didática com Arduino + interface gráfica MATLAB para controle de velocidade de motor CC. Apresenta fabricação, arranjo do motor, circuitos de potência e controle.

| Aspecto | Segundo et al. (2019) | Girino |
|---|---|---|
| Microcontrolador | Arduino | ESP8266 WROOM |
| Interface | MATLAB GUI | **Web embarcada** |
| Conectividade | USB | **Wi-Fi + OTA** |
| Contexto | Graduação em engenharia | Graduação em engenharia |

**Pontos fortes:** Publicado em congresso SBA (relevante), demonstração prática completa.
**Lacunas:** Dependência MATLAB, sem conectividade sem fio.

---

### 1.4 MotoShield (Takács et al., 2021)

**Veículo:** IEEE EDUCON
**DOI:** https://ieeexplore.ieee.org/document/9453979

**Descrição:** Shield Arduino miniaturizado com motor DC + encoder incremental. Open-source com biblioteca para IDE Arduino. Exemplos de controle PID. Design compacto para "pocket labs".

| Aspecto | MotoShield | Girino |
|---|---|---|
| Forma | Shield Arduino R3 | PCB independente |
| MCU | Arduino UNO/Mega | ESP8266 WROOM |
| Conectividade | Nenhuma | **Wi-Fi** |
| Interface | Arduino IDE serial | **Web embarcada** |
| OTA | Não | **Sim** |
| API | C/C++ library | **REST (HTTP)** |
| Citação | 8 citações | — |

**Pontos fortes:** Projeto maduro, hardware integrado, publicado em IEEE, comunidade ativa.
**Lacunas:** Sem conectividade, sem interface web, sem OTA.

---

### 1.5 OpenMCT (Von Chong, 2026)

**Veículo:** HardwareX (Elsevier)
**DOI:** https://www.sciencedirect.com/science/article/pii/S2468067226000544

**Descrição:** Kit educacional open-source para controle de motor DC. Teensy 4 + encoder incremental + H-bridge + sensor de corrente. GUI Python/Qt com telemetria, logging, sintonia PID e controle no domínio z. Certificado OSHWA.

| Aspecto | OpenMCT | Girino |
|---|---|---|
| MCU | Teensy 4.x | ESP8266 WROOM |
| Encoder | Incremental | LPD3806-600BM |
| GUI | Python/Qt (desktop) | **Web (navegador)** |
| Conectividade | USB | **Wi-Fi** |
| OTA | Não | **Sim** |
| Certificação | OSHWA | Planejado |
| Maturidade | Alta (2026) | Inicial |
| Software necessário | Python + Qt | **Nenhum** |

**Pontos fortes:** Projeto mais maduro e completo, certificado OSHWA, GUI rica, controle no domínio z.
**Lacunas:** Requer instalação de Python + Qt, sem Wi-Fi, sem OTA, sem web.

---

### 1.6 Reck & Sreenivas (2015, 2016) — Papers Fundacionais

**Veículos:** ACC (IEEE), Electronics (MDPI)
**DOI:** https://ieeexplore.ieee.org/document/7171014 e https://www.mdpi.com/2079-9292/5/3/43

**Descrição:** Kit portátil "take-home" com motor DC + caixa de redução + encoder. Compara Arduino, Raspberry Pi e DAQ comercial. Demonstração de controle PID de posição. 97 citações combinadas.

| Aspecto | Reck & Sreenivas | Girino |
|---|---|---|
| MCU | Arduino / RPi | ESP8266 |
| Motor | DC + gearbox | DC |
| Encoder | Sim | Sim |
| PID | Posição e velocidade | Velocidade (planejado) |
| Conectividade | USB / Ethernet | **Wi-Fi nativo** |
| Portabilidade | Kit take-home | **Kit take-home + web** |
| Avaliação pedagógica | **Sim (completa)** | A fazer |

**Pontos fortes:** Papers fundacionais do campo, avaliação pedagógica formal com estudantes, custo detalhado.
**Lacunas:** Sem Wi-Fi nativo, sem web embarcada, sem OTA.

---

### 1.7 TCLab — Temperature Control Lab (Hedengren et al., 2020+)

**Veículo:** Multiple (19+ papers)
**URL:** https://apmonitor.com/pdc/index.php/Main/ArduinoTemperatureControl

**Descrição:** Laboratório de controle de temperatura em Arduino Leonardo. Dois aquecedores, dois sensores. Suporte Python/MATLAB/Simulink. Adotado mundialmente. Modelo de sucesso em publicação de plataforma educacional.

| Aspecto | TCLab | Girino |
|---|---|---|
| Variável controlada | Temperatura | Velocidade/posição angular |
| MCU | Arduino Leonardo | ESP8266 |
| Software | Python/MATLAB | **Nenhum (navegador)** |
| Conectividade | USB | **Wi-Fi** |
| Publicações | **19+ papers** | 0 |
| Adoção | Mundial | — |

**Pontos fortes:** Modelo de sucesso em publicação, comunidade grande, materiais didáticos completos.
**Lacunas:** Variável diferente (temperatura vs motor), sem Wi-Fi, requer Python ou MATLAB.

**Nota:** O TCLab é o **modelo a seguir** para estratégia de publicação — mostrar como uma plataforma open-source pode gerar dezenas de papers e ser adotada globalmente.

---

## 2. Tabela Comparativa Geral

| Característica | Cabral 2025 | Alexandre 2025 | Segundo 2019 | MotoShield 2021 | OpenMCT 2026 | Reck 2015 | TCLab 2020 | **Girino** |
|---|---|---|---|---|---|---|---|---|
| Motor DC | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | — | **✅** |
| Encoder | ✅ | ✅ | — | ✅ | ✅ | ✅ | — | **✅** |
| PID | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | **Planejado** |
| Microcontrolador | Arduino | Arduino | Arduino | Arduino | Teensy 4 | Arduino/RPi | Arduino Leo | **ESP8266** |
| Wi-Fi nativo | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | **✅** |
| Interface web | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | **✅** |
| API REST | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | **✅** |
| OTA firmware | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | **✅** |
| Sem software externo | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | **✅** |
| Open-source HW | Parcial | ❌ | ❌ | ✅ | ✅ | ✅ | ✅ | **✅** |
| Modelagem matemática | ✅ | — | — | — | ✅ | ✅ | ✅ | **A fazer** |
| Avaliação com alunos | — | — | — | — | — | ✅ | ✅ | **A fazer** |
| Custo (< US$ 20) | ✅ | ✅ | ✅ | — | — | ❌ | ✅ | **✅** |
| Contexto brasileiro | ✅ | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ | **✅** |

---

## 3. Análise de Lacunas (Gap Analysis)

### O que todos os trabalhos têm em comum:
1. Motor DC + encoder como planta
2. Microcontrolador como controlador
3. Foco em ensino de controle
4. Baixo custo

### O que nenhum trabalho oferece:
1. **Conectividade Wi-Fi nativa** — Todos usam Arduino UNO/Mega/Teensy sem Wi-Fi
2. **Interface web embarcada** — Todos dependem de MATLAB, Python, LabVIEW ou aplicativo desktop
3. **OTA firmware updates** — Nenhum permite atualizar o firmware sem fio
4. **API REST** — Nenhum oferece interface HTTP para integração
5. **Zero instalação de software** — Todos exigem que o aluno instale algo

### O que o Girino ainda precisa desenvolver:
1. **Modelagem matemática** do sistema motor + encoder
2. **Implementação do PID** com sintonia
3. **Avaliação pedagógica** com alunos
4. **Comparação experimental** simulação vs hardware

---

## 4. Diferenciais do Girino para o Artigo

### Argumento Central

> As plataformas existentes para ensino de controle com motor DC compartilham uma limitação fundamental: **a dependência de software proprietário (MATLAB) ou instalação local (Python, LabVIEW)** para interação com o hardware. Isso cria barreiras de acessibilidade, especialmente em contextos onde alunos não têm acesso a licenças acadêmicas ou computadores pessoais.
>
> O Girino propõe uma mudança de paradigma: **o navegador web como interface universal**. Com ESP8266 e servidor web embarcado, o aluno interage com o motor via qualquer dispositivo com navegador — celular, tablet, Chromebook — sem instalar nada. A atualização OTA permite que o professor atualize o firmware de todas as bancadas remotamente.

### Contribuições Específicas

| # | Contribuição | Novidade |
|---|---|---|
| 1 | ESP8266 como plataforma para ensino de controle | Primeiro uso documentado no contexto |
| 2 | Interface web embarcada para controle de motor | Nenhum trabalho anterior oferece |
| 3 | API REST para experimentação de controle | Abre possibilidades de automação e integração |
| 4 | OTA para gestão de bancadas de laboratório | Facilita manutenção em escala |
| 5 | Zero instalação de software | Democratiza o acesso ao laboratório |
| 6 | Licença tripla open-source | Garante reprodutibilidade e colaboração |

---

## 5. Referências da RBEF e Periódicos Brasileiros

### Papers na RBEF com uso de microcontroladores (contexto de apoio)

| # | Título | Autores | Ano | DOI | Relevância |
|---|--------|---------|-----|-----|---|
| 1 | Determinación del rendimiento de un motor de Stirling usando Arduino | Savall-Alemany et al. | 2020 | https://doi.org/10.1590/1806-9126-RBEF-2020-0279 | Arduino + sensores em motor. Mostra abordagem de baixo custo. |
| 2 | Potência e força eletromotriz em um gerador didático de corrente alternada | Alves et al. | 2022 | https://doi.org/10.1590/1806-9126-RBEF-2021-0379 | Motor com controle de rotação. Medição de EMF. |
| 3 | Uma aula sobre conversão de energia utilizando bicicleta, motor, alternador e lâmpada | Borges, Dickman, Vertchenko | 2018 | https://doi.org/10.1590/1806-9126-RBEF-2017-0215 | Motor em experimento didático de física. |
| 4 | Motor elétrico — SimuFísica® | Souza, Oliveira, Luiz | 2024 | https://doi.org/10.1590/1806-9126-RBEF-2023-0219 | Simulador de motor para ensino. Equações e dinâmica. |
| 5 | Sistema automatizado para medición del coeficiente de fricción estática | González-Laprea, Santiago | 2021 | https://doi.org/10.1590/1806-9126-RBEF-2021-0056 | Arduino + motor + sensores para ensino de física. |
| 6 | A placa Arduino: uma opção de baixo custo para experiências de física | Souza et al. | 2011 | https://doi.org/10.1590/S1806-11172011000100026 | Paper fundacional Arduino na RBEF. |
| 7 | Física com Arduino para iniciantes | Cavalcante et al. | 2011 | https://doi.org/10.1590/S1806-11172011000400018 | Arduino para automação e aquisição de dados. |
| 8 | Strain and deformation measurement using Arduino | Silva et al. | 2019 | https://doi.org/10.1590/1806-9126-RBEF-2018-0206 | Aquisição com Arduino e condicionamento de sinal. |
| 9 | Kit experimental com Arduino para ensino de Física Moderna | Silveira, Girardi | 2017 | https://doi.org/10.1590/1806-9126-RBEF-2016-0287 | Kit de baixo custo com interface web. |
| 10 | Física experimental com Arduino: ondas em uma corda | Sousa Jr. et al. | 2020 | https://doi.org/10.1590/1806-9126-RBEF-2020-0177 | Técnicas de otimização de ADC e timing. |
| 11 | Kit experimental com Arduino para oscilações em tempo real | Matos Pereira, da Silva | 2021 | https://doi.org/10.1590/1806-9126-RBEF-2021-0186 | Aquisição e visualização em tempo real. |
| 12 | Práticas experimentais de Física a distância: Millikan com Arduino | Barros, Dias | 2019 | https://doi.org/10.1590/1806-9126-RBEF-2019-0049 | **Controle remoto de experimento via web.** Filosofia similar ao Girino. |
| 13 | Sismógrafo empregando sensores piezoelétricos em Arduino | Amorim et al. | 2021 | https://doi.org/10.1590/1806-9126-RBEF-2021-0267 | Aquisição de dados com Arduino. |

### Revisões sistemáticas brasileiras sobre Arduino no ensino

| # | Título | Autores | Ano | URL |
|---|--------|---------|-----|-----|
| 14 | Contribuições do Arduino no Ensino de Física: revisão sistemática | — | ~2018 | https://bia.ifpi.edu.br/jspui/handle/123456789/4839 |
| 15 | Arduino no Ensino de Física: Revisão Sistemática de Literatura | UFPA | ~2022 | https://www.periodicos.ufpa.br/index.php/revistaamazonia/article/view/12175 |

---

## 6. Estratégia de Publicação Recomendada

### Opção A: RBEF (Revista Brasileira de Ensino de Física)
- **Vantagem:** Lacuna clara — nenhum paper sobre motor + encoder + controle. Público amplo de físicos educadores.
- **Desafio:** Precisa de enfoque em física (não apenas engenharia). Argumentar que controle é relevante para física moderna.
- **Ângulo:** "Plataforma de baixo custo para ensino de controle e automação via navegador web"

### Opção B: COBENGE (Congresso Brasileiro de Educação em Engenharia)
- **Vantagem:** Foco direto em educação em engenharia. Edição 2026 em Belo Horizonte.
- **Desafio:** Congresso (não periódico). Pode ser stepping stone para artigo em periódico.

### Opção C: CBA (Congresso Brasileiro de Automática)
- **Vantagem:** Já publicou trabalhos similares (Sousa 2022, Alves 2024). Comunidade de controle.
- **Desafio:** Público técnico, precisa de modelagem matemática e resultados experimentais.

### Opção D: RBEE (Revista Brasileira de Educação em Engenharia)
- **Vantagem:** Periódico direto de ABENGE. Foco em educação.
- **Recomendação:** Ideal para artigo completo com avaliação pedagógica.

### Estratégia sugerida:
1. **Curto prazo:** Submeter ao COBENGE 2026 ou CBA (paper de 6-8 páginas)
2. **Médio prazo:** Submeter artigo completo à RBEF ou RBEE com avaliação pedagógica
3. **Longo prazo:** Submeter versão estendida ao IEEE EDUCON ou HardwareX
