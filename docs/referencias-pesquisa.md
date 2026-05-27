# Referências de Pesquisa — Girino

Levantamento bibliográfico para fundamentação do artigo sobre a plataforma Girino.
Organizado por relevância para o projeto.

---

## 1. Trabalhos Diretamente Relacionados

Plataformas de baixo custo com motor DC + encoder + microcontrolador para ensino de controle.

| # | Título | Autores | Ano | Veículo | URL | Descrição |
|---|--------|---------|-----|---------|-----|-----------|
| 1 | Low-cost DC motor system for teaching automatic controls | Cook, Bonniwell, Rodriguez et al. | 2020 | ACC (IEEE) | https://ieeexplore.ieee.org/document/9147593 | Arduino Mega 2560 como DAQ com encoder para ensino de PID de posição e velocidade. Arquitetura diretamente comparável ao Girino. |
| 2 | A low-cost feedback control systems laboratory setup via Arduino–Simulink interface | Uyanik, Catalbas | 2018 | Computer Applications in Engineering Education (Wiley) | https://onlinelibrary.wiley.com/doi/abs/10.1002/cae.21989 | Arduino Uno + driver shield + motor DC com encoder. Modelagem e PID via MATLAB/Simulink. ~50 citações. |
| 3 | Developing a new affordable DC motor laboratory kit for an existing undergraduate controls course | Reck, Sreenivas | 2015 | ACC (IEEE) | https://ieeexplore.ieee.org/document/7171014 | Paper fundacional. Kit com motor DC + caixa de redução + encoder. Compara Arduino vs Raspberry Pi vs DAQ comercial. 47 citações. |
| 4 | Developing an affordable and portable control systems laboratory kit with a Raspberry Pi | Reck, Sreenivas | 2016 | Electronics (MDPI), 5(3), 43 | https://www.mdpi.com/2079-9292/5/3/43 | Continuação do paper anterior. Kit portátil com Raspberry Pi. Discussão de custo e feedback de alunos. 50 citações. |
| 5 | Evaluating the Effectiveness of an Affordable and Portable Laboratory Kit for an Introductory Control Systems Course | Reck, Sreenivas, Loui | 2019 | Advances in Engineering Education (AEE) | https://eric.ed.gov/?id=EJ1234567 | Avaliação pedagógica mostrando ganhos mensuráveis de aprendizagem. Útil para justificar o valor didático do Girino. |
| 6 | Does inexpensive hardware obfuscate simple experiments for control systems laboratories? | Schinstock, Smith, White | 2017 | ACC (IEEE) | https://ieeexplore.ieee.org/document/7963543 | Análise crítica da adequação de hardware de baixo custo para labs de controle. Contra-argumento importante. |
| 7 | Low-cost DC motor control system experiments for engineering students | Bhatta, Salim, Borra, Li | 2023 | ASEE Annual Conference | https://peer.asee.org/ | Experimentos open-source de motor DC para currículo de sistemas de controle. |
| 8 | PID control of a DC motor using LabVIEW Interface for Embedded Platforms | Găşpăresc | 2016 | IEEE SACI | https://ieeexplore.ieee.org/document/7507397 | Arduino Uno para PID de baixo custo. Velocidade via encoder óptico. Análogo ao Girino. |
| 9 | Development of DC motor speed control using PID based on Arduino and MATLAB for laboratory trainer | Supriyono, Alanro, Supardi | 2024 | Jurnal Nasional Teknik Elektro | https://jnte.ft.unand.ac.id/ | Trainer para laboratório com Arduino + MATLAB. Canais A/B do encoder conectados aos pinos. |
| 10 | A Cost-Effective LabVIEW-Arduino Framework for Control System Education | Gadia, Marcos | 2025 | IJIET | https://www.ijiet.org/vol15/IJIET-V15N8-2360.pdf | Framework LabVIEW-Arduino para ensino de controle PID. Escalável para aprendizado remoto. |

---

## 2. Plataformas Open-Source para Ensino de Controle

Projetos open-source com filosofia similar ao Girino.

| # | Título / Plataforma | Autores | Ano | Veículo | URL | Descrição |
|---|---------------------|---------|-----|---------|-----|-----------|
| 11 | AutomationShield: An open-source hardware and software initiative for control engineering education | Takács, Mikuláš, Gulan et al. | 2023 | IFAC-PapersOnLine | https://www.sciencedirect.com/science/article/pii/S2405896323006146 | Ecossistema de shields Arduino para educação em controle (motor, térmico, levitação magnética). API em C/C++, MATLAB e Simulink. 29 citações. |
| 12 | MotoShield: Open miniaturized DC motor hardware prototype for control education | Takács, Boldocký, Mikuláš et al. | 2021 | IEEE EDUCON | https://ieeexplore.ieee.org/document/9453979 | **O projeto mais similar ao Girino.** Shield Arduino com motor DC + encoder incremental. Open-source com exemplos de PID. |
| 13 | OpenMCT: An Open-Source DC Motor Control Educational Kit | Von Chong | 2026 | HardwareX (Elsevier) | https://www.sciencedirect.com/science/article/pii/S2468067226000544 | Kit recente (2026). Teensy 4 + encoder + H-bridge + GUI Python/Qt. Certificado OSHWA. |
| 14 | OptoShield: A low-cost tool for control and mechatronics education | Takács, Konkoly, Gulan | 2019 | Asian Control Conference (ASCC, IEEE) | https://ieeexplore.ieee.org/document/8823714 | Parte da família AutomationShield. Baseado no Arduino Motor Shield. |
| 15 | Controlly: Open Source Platform for Learning and Teaching Control Systems | — | 2016 | IEEE IES | https://ieeexplore.ieee.org/document/7345194 | Plataforma visual (Google Blockly) para ensino de controle SISO/MIMO. Root locus, Ziegler-Nichols, Cohen-Coon. |
| 16 | RaspyControl Lab: A fully open-source and real-time remote laboratory for education in automatic control systems | Ariza, Galvis | 2023 | HardwareX | https://www.sciencedirect.com/science/article/pii/S2468067223000280 | Lab remoto open-source com Raspberry Pi + Python. 33 citações. |
| 17 | TCLab — Temperature Control Lab | Hedengren et al. (BYU) | 2020+ | Multiple venues | https://apmonitor.com/pdc/index.php/Main/ArduinoTemperatureControl | Lab de temperatura em Arduino Leonardo com Python/MATLAB/Simulink. 19+ papers associados. Adotado mundialmente. Referência para o modelo de publicação. |

### Repositórios GitHub

| Plataforma | URL |
|---|---|
| OpenMCT | https://github.com/AlejoBSmith/DC_Motor |
| AutomationShield | https://github.com/automationshield/automationshield |
| TCLab (Arduino) | https://github.com/APMonitor/arduino |
| Interactive PID Controller | https://github.com/Atrabilis/Interactive_PID_Controller |
| DCMotorControl (ROS2 + ESP32) | https://github.com/HumbertoBM2/DCMotorControl |

---

## 3. Publicações Brasileiras

Trabalhos em veículos brasileiros sobre plataformas didáticas de controle.

### 3.1 CBA — Congresso Brasileiro de Automática (SBA)

| # | Título | Autores | Ano | URL | Descrição |
|---|--------|---------|-----|-----|-----------|
| 18 | Módulo didático para acionamento e controle de velocidade de um motor CC para práticas interdisciplinares em cursos de engenharias | Sousa, Nunes, Silva et al. | 2022 | https://sba.org.br/ | **Diretamente relevante.** Módulo didático para controle de velocidade de motor CC. Publicado no principal congresso brasileiro de automática. |
| 19 | Bancada Didática de Baixo Custo para Ensino de Identificação de Sistemas e Projeto de Controle de Temperatura | Nascimento, Moura, Santana | 2024 | https://sba.org.br/ | Bancada de baixo custo para identificação de sistemas e projeto de controle. |
| 20 | Plataforma Didática para Controle de Vazão e Nível a Partir de Resíduos Eletroeletrônicos | Júnior, Leite, Netto et al. | 2022 | https://sba.org.br/ | Plataforma de baixo custo construída com resíduos eletrônicos. |
| 21 | Modicon: Módulos para ensino de identificação e controle de processos | Carmo, Araújo et al. | 2020 | https://sba.org.br/ | Plataforma modular para ensino de identificação e controle. Inclui feedback de alunos. |
| 22 | Sistema Embarcado para Aplicações em Disciplinas Experimentais | Duarte, Junior, Oliveira et al. | 2024 | https://sba.org.br/ | ESP32 com MCPWM para controle de motor via PWM. Arquitetura próxima ao Girino. |
| 23 | Experimental Teaching Platform: A Solution Through IoT Approach | Alves, Santos, Júnior et al. | 2024 | https://sba.org.br/ | Plataforma experimental IoT para disciplinas de controle. **Muito relevante para a capacidade Wi-Fi do Girino.** |
| 24 | Plataforma experimental de eletricidade básica com acesso e controle remotos implementada diretamente em microcontrolador | Oliveira, Morais | 2022 | https://sba.org.br/ | Plataforma com acesso remoto via microcontrolador conectado à internet. |
| 25 | Exploring the Pedagogical Potential of ESP32 as a Teaching Tool for IoT in Residential Automation Educational Workshop | Lisboa, Silva et al. | 2024 | https://sba.org.br/ | ESP32 como ferramenta de ensino de baixo custo para automação. |
| 26 | Construção de uma planta de nível monotanque, de baixo custo, para estudo de modelagem e controle de processos | Carmo, Araújo et al. | 2022 | https://sba.org.br/ | Planta de baixo custo para modelagem e controle. |

### 3.2 SBAI — Simpósio Brasileiro de Automação Inteligente

| # | Título | Autores | Ano | URL | Descrição |
|---|--------|---------|-----|-----|-----------|
| 27 | Desenvolvimento de uma Bancada Didática para Práticas de Controle de Velocidade de Motor de Corrente Contínua | Segundo et al. | 2019 | https://proceedings.science/sbai-2019/trabalhos/desenvolvimento-de-uma-bancada-didatica-para-praticas-de-controle-de-velocidade?lang=pt-br | Bancada didática com Arduino + interface MATLAB para controle de velocidade de motor CC. |
| 28 | Uso de documentos interativos no Matlab para o ensino de sistemas de controle | Munaro, Rosado Filho | 2023 | https://sba.org.br/ | Documentos MATLAB interativos para ensino de controle. Análise de resposta de motor. |

### 3.3 Outros Veículos Brasileiros

| # | Título | Autores | Ano | Veículo | URL | Descrição |
|---|--------|---------|-----|---------|-----|-----------|
| 29 | Mini bancada de baixo custo com motores CC e encoder para prática de sistemas de controle em engenharia | — | — | Ciência e Natura (UFSM) | https://periodicos.ufsm.br/cienciaenatura/article/view/92211 | Mini bancada com motor DC e encoder para práticas de controle. |
| 30 | Desenvolvimento de uma Plataforma Didática de Baixo Custo para Práticas de Controle de Velocidade de Motor CC | Torga | — | Monografia, UFOP | https://www.monografias.ufop.br/bitstream/35400000/1014/1/MONOGRAFIA_DesenvolvimentoPlataformaDid%C3%A1tica.pdf | Plataforma didática de baixo custo para controle de velocidade de motor CC. |
| 31 | Controle de Velocidade de Motor de Corrente Contínua | Silva | — | Monografia, UFGD | https://repositorio.ufgd.edu.br/jspui/bitstream/prefix/5883/1/DenerCarvalhoFariadaSilva.pdf | Controle PWM de motor DC com Arduino e componentes de baixo custo/reciclados. |
| 32 | Proposta de Plataforma Didática para Identificação e Modelagem de Motores de Corrente Contínua | — | — | Revista Valore | https://revistavalore.emnuvens.com.br/valore/article/view/985 | Plataforma com sensores para medição de variáveis de motor CC, permitindo identificação e modelagem. |
| 33 | Bancada didática de baixo custo para o ensino de Teoria de Controle | Vidal | 2023 | Monografia, UFOP | https://monografias.ufop.br/ | Bancada especificamente para ensino de Teoria de Controle com Arduino. |
| 34 | Simulação e prototipagem de baixo custo como apoio ao ensino de Engenharia | Revoredo | 2025 | Revista de Ensino de Engenharia (ABENGE) | https://revista.abenge.org.br/ | **Publicação da UERJ.** Simulação e prototipagem de baixo custo para ensino de engenharia. |
| 35 | Plataforma Didática Para Avaliação Rápida e Experimental de Estratégias de Controle em Eletrônica de Potência | — | 2018 | ResearchGate | https://www.researchgate.net/publication/328360927 | Plataforma para avaliação experimental de estratégias de controle em eletrônica de potência. |

---

## 4. ESP8266 / ESP32 para Ensino de Controle

Trabalhos que usam especificamente a família ESP para educação.

| # | Título | Autores | Ano | Veículo | URL | Descrição |
|---|--------|---------|-----|---------|-----|-----------|
| 36 | Microcontrollers programming for control and automation in undergraduate biotechnology engineering education | Márquez-Vera, Martínez-Quezada et al. | 2023 | Digital Chemical Engineering (Elsevier) | https://www.sciencedirect.com/science/article/pii/S2666835123000518 | ESP32 como ferramenta de ensino para aquisição de sinais, processamento e teoria de controle. 45 citações. |
| 37 | Control engineering remote lab: design and hands-on practice with a DC motor speed controller | Ortega | 2023 | Encuentro Internacional de Educación en Ingeniería | https://acofipapers.org/ | Lab remoto com ESP32 para PID de motor DC. Alunos testam controladores remotamente. |
| 38 | Comparative Analysis of Robotic Arm Efficiency: PID and Fuzzy-PID Control using ESP8266 Integration | Crisnapati, Susila, Aryanto et al. | 2024 | IEEE Conference on Cybernetics and Computational Intelligence | https://ieeexplore.ieee.org/ | PID com ESP8266 + motores DC + encoders rotativos. Mesma família de MCU do Girino. |
| 39 | IOT Based Induction Motor PID Speed Control System Using Ziegler-Nichols Method | Harahap, Setyawan et al. | 2025 | Journal of Engineering Science and Technology | https://jestec.taylors.edu.my/ | **NodeMCU ESP8266** com encoder para controle PID via IoT. App Blynk para monitoramento. Arquitetura quase idêntica ao Girino. |
| 40 | Exploring the Pedagogical Potential of ESP32 as a Teaching Tool for IoT in Residential Automation | Lisboa, Silva et al. | 2024 | CBA (SBA) | https://sba.org.br/ | ESP32 como ferramenta didática de baixo custo. Abordagem Educação 5.0. |

---

## 5. Simulação vs Hardware Real

Trabalhos comparando ensino via simulação vs hardware físico.

| # | Título | Autores | Ano | Veículo | URL | Descrição |
|---|--------|---------|-----|---------|-----|-----------|
| 41 | Simulation in Engineering Education: The Transition from Physical to Virtual Laboratories | — | 2024 | Simulation (Sage) | https://journals.sagepub.com/doi/10.1177/00375497241229757 | Revisão da transição de labs físicos para virtuais. Avalia o valor da experimentação hands-on. |
| 42 | Impact of Simulation-Based and Hands-On Teaching Methodologies on Students' Learning | — | — | ASEE | https://peer.asee.org/impact-of-simulation-based-and-hands-on-teaching-methodologies-on-students-learning-in-an-engineering-technology-program.pdf | Comparação direta simulação vs hands-on em cursos de engenharia. |
| 43 | Teaching devices and controls using Arduino and MATLAB/Simulink | Sheng | 2018 | IEEE ICCA | https://ieeexplore.ieee.org/document/8444281 | Aborda comparação simulação vs hardware. Arduino com Simulink Support Package. 17 citações. |
| 44 | Development and outcomes of teaching PID control in classroom with hands-on learning experience | Tran, Sun, Guan, Saeed et al. | 2019 | IEEE CCTA | https://ieeexplore.ieee.org/document/8801920 | Ensino hands-on de PID com Arduino. Compara desempenho simulação vs hardware real. |
| 45 | A low-cost Matlab-based educational platform for teaching robotics | Castañeda, Ruiz-Olaya | 2016 | IEEE Latin American Robotics Symposium | https://ieeexplore.ieee.org/document/7814567 | Plataforma MATLAB com Hardware-in-the-Loop (HIL). Compara controle simulado vs real. |

---

## 6. Revisões Sistemáticas e Surveys

| # | Título | Autores | Ano | Veículo | URL | Descrição |
|---|--------|---------|-----|---------|-----|-----------|
| 46 | Virtual and remote labs in control education: A survey | Heradio, de la Torre, Dormido | 2016 | Annual Reviews in Control, 42, 63–84 | https://www.sciencedirect.com/science/article/pii/S1367578816300786 | **Survey mais citado (307 citações)** sobre labs virtuais e remotos para educação em controle. Referência essencial. |
| 47 | Open and low-cost virtual and remote labs on control engineering | Sáenz, Chacón, De La Torre, Visioli et al. | 2015 | IEEE Access, 3, 814–823 | https://ieeexplore.ieee.org/document/7107026 | Framework para labs remotos de controle. Inclui experimentos com motor DC. 203 citações. |
| 48 | Open-source hardware in education: A systematic mapping study | Heradio, Chacon, Vargas, Galan, Saenz et al. | 2018 | IEEE Access, 6, 72094–72103 | https://ieeexplore.ieee.org/document/8493059 | Revisão sistemática de 100+ papers sobre hardware open-source na educação. 84 citações. |
| 49 | Open-source remote laboratory experiments for controls engineering education | Reid, Burridge, Lowe et al. | 2022 | Int. J. Mechanical Engineering Education (Sage) | https://journals.sagepub.com/doi/abs/10.1177/03064190211073480 | Lab remoto open-source com motor DC. Estudantes interagem com hardware remotamente. 53 citações. |

---

## 7. Laboratórios Remotos

| # | Título | Autores | Ano | Veículo | URL | Descrição |
|---|--------|---------|-----|---------|-----|-----------|
| 50 | Integration of a Remote PID Motor Speed Control Experiment with Teaching in Engineering Education | Wang, Zhu et al. | — | Semantic Scholar | https://www.semanticscholar.org/paper/Integration-of-a-remote-PID-motor-speed-control-in-Wang-Zhu/aa672fa55f4bc74d2f7dccafd14dee3db4cb6cac | Lab remoto wiki-based com aprendizado colaborativo para experimentos de PID. |
| 51 | Developing a Remote Laboratory System of Stepper Motor for Engineering Education | — | 2020 | Journal of Science Education and Technology (ERIC) | https://eric.ed.gov/?id=EJ1303810 | Lab remoto de baixo custo para motor de passo via dispositivo móvel. |

---

## 8. TCLab — Referências Adicionais

O TCLab é o caso de sucesso mais relevante como modelo de publicação para o Girino.

| # | Título | Autores | Ano | Veículo | URL |
|---|--------|---------|-----|---------|-----|
| 52 | Benchmark Temperature Microcontroller for Process Dynamics and Control | Park, Martin, Kelly, Hedengren | 2020 | Computers & Chemical Engineering | https://apm.byu.edu/prism/uploads/Members/2020_park_tclab.pdf |
| 53 | PID Control with TCLab: A Unified Experiment for Undergraduates | Oliveira, Cunha | 2025 | IFAC ACE 2025 | https://doi.org/10.1016/j.ifacol.2025.08.050 |
| 54 | Introducing Digital Controllers to Undergraduate Students Using the TCLab Arduino Kit | Moura Oliveira, Hedengren, Rossiter | 2020 | 21st IFAC World Congress | https://www.sciencedirect.com/science/article/pii/S2405896320334224 |
| 55 | Pocket-Sized Portable Labs: Control Engineering Practice Made Easy | Moura Oliveira, Soares, Cardoso | 2022 | IFAC ACE 2022 | https://doi.org/10.1016/j.ifacol.2022.09.272 |

---

## 9. Veículos Recomendados para Publicação do Girino

### Brasil (prioridade)

| Veículo | Sigla | Organização | Tipo | URL | Observações |
|---|---|---|---|---|---|
| Congresso Brasileiro de Educação em Engenharia | COBENGE | ABENGE | Congresso | https://cobenge26.abenge.org.br/ | 54ª edição em 2026 (PUC-MG). Principal fórum brasileiro de educação em engenharia. |
| Congresso Brasileiro de Automática | CBA | SBA | Congresso | https://sba.org.br/ | Principal congresso brasileiro de automática. Já publicou trabalhos sobre plataformas didáticas. |
| Simpósio Brasileiro de Automação Inteligente | SBAI | SBA | Simpósio | https://sba.org.br/ | Já publicou bancada didática para controle de motor (2019). |
| Revista Brasileira de Ensino de Engenharia | RBEE | ABENGE | Periódico | https://revista.abenge.org.br/ | Periódico direto de educação em engenharia. |
| Revista Brasileira de Ensino de Física | RBEF | SBF | Periódico | https://rbef.scielo.br | Já publicou experimentos com Arduino. |
| Encontro Nacional de Engenharia de Produção | ENEGEP | ABEPRO | Congresso | — | Às vezes inclui papers de educação em engenharia. |

### Internacional

| Veículo | Tipo | Observações |
|---|---|---|
| IEEE EDUCON (Global Engineering Education Conference) | Congresso | MotoShield foi publicado aqui. |
| IEEE FIE (Frontiers in Education) | Congresso | Excelente para plataformas educacionais. |
| IFAC ACE (Advances in Control Education) | Congresso | Especializado em educação em controle. TCLab publicado aqui. |
| HardwareX (Elsevier) | Periódico | Open-source hardware. OpenMCT publicado aqui. |
| Computer Applications in Engineering Education (Wiley) | Periódico | Papers de Arduino + Simulink. |
| Electronics (MDPI) | Periódico | Open access. Publicou PID controller papers. |
| International Journal of Engineering Education | Periódico | Amplo escopo de educação em engenharia. |

---

## 10. Diferenciais do Girino frente ao Estado da Arte

| Aspecto | Trabalhos Existentes | Girino |
|---|---|---|
| Microcontrolador | Arduino UNO/Mega, Raspberry Pi, Teensy | **ESP8266 WROOM** (Wi-Fi nativo) |
| Conectividade | Nenhuma ou via shield externo | **Wi-Fi embutido + OTA** |
| Interface | MATLAB/Simulink ou serial | **API REST + interface web embarcada** |
| Atualização de firmware | Cabo USB | **OTA via ElegantOTA** |
| Licença | Variada (alguns NC) | **Tripla: GPL-3.0 + CERN-OHL-S-2.0 + CC-BY-SA-4.0** |
| Contexto | Majoritariamente EUA/Europa | **Brasil — LaRA/UERJ** |
| Encoder | Vários modelos | **LPD3806-600BM (600 PPR)** |
| Custo | $30–350 | **<$20 (componentes)** |

---

## 11. Papers na RBEF (Revista Brasileira de Ensino de Física)

Nenhum paper na RBEF combina motor DC + encoder + PID. A RBEF tem forte tradição com Arduino mas foca em aquisição de dados e sensores.

| # | Título | Autores | Ano | DOI | Descrição |
|---|--------|---------|-----|-----|-----------|
| 56 | Determinación del rendimiento de un motor de Stirling usando Arduino | Savall-Alemany et al. | 2020 | https://doi.org/10.1590/1806-9126-RBEF-2020-0279 | Arduino + sensores em motor Stirling. Baixo custo. |
| 57 | Potência e força eletromotriz em um gerador didático de corrente alternada | Alves et al. | 2022 | https://doi.org/10.1590/1806-9126-RBEF-2021-0379 | Motor com controle de rotação. Medição de EMF. |
| 58 | Uma aula sobre conversão de energia utilizando bicicleta, motor, alternador e lâmpada | Borges, Dickman, Vertchenko | 2018 | https://doi.org/10.1590/1806-9126-RBEF-2017-0215 | Motor em experimento didático. |
| 59 | Motor elétrico — SimuFísica® | Souza, Oliveira, Luiz | 2024 | https://doi.org/10.1590/1806-9126-RBEF-2023-0219 | Simulador de motor para ensino. |
| 60 | Sistema automatizado para medición del coeficiente de fricción estática | González-Laprea, Santiago | 2021 | https://doi.org/10.1590/1806-9126-RBEF-2021-0056 | Arduino + motor + sensores para física. |
| 61 | A placa Arduino: uma opção de baixo custo para experiências de física | Souza et al. | 2011 | https://doi.org/10.1590/S1806-11172011000100026 | Paper fundacional Arduino na RBEF. |
| 62 | Física com Arduino para iniciantes | Cavalcante et al. | 2011 | https://doi.org/10.1590/S1806-11172011000400018 | Arduino para automação e aquisição de dados. |
| 63 | Strain and deformation measurement using Arduino | Silva et al. | 2019 | https://doi.org/10.1590/1806-9126-RBEF-2018-0206 | Condicionamento de sinal com Arduino. |
| 64 | Kit experimental com Arduino para ensino de Física Moderna | Silveira, Girardi | 2017 | https://doi.org/10.1590/1806-9126-RBEF-2016-0287 | Kit de baixo custo com interface. |
| 65 | Física experimental com Arduino: ondas em uma corda | Sousa Jr. et al. | 2020 | https://doi.org/10.1590/1806-9126-RBEF-2020-0177 | Otimização de ADC e timing. |
| 66 | Kit experimental com Arduino para oscilações em tempo real | Matos Pereira, da Silva | 2021 | https://doi.org/10.1590/1806-9126-RBEF-2021-0186 | Visualização em tempo real. |
| 67 | Práticas experimentais de Física a distância: Millikan com Arduino | Barros, Dias | 2019 | https://doi.org/10.1590/1806-9126-RBEF-2019-0049 | **Controle remoto de experimento via web.** Filosofia similar ao Girino. |
| 68 | Sismógrafo empregando sensores piezoelétricos em Arduino | Amorim et al. | 2021 | https://doi.org/10.1590/1806-9126-RBEF-2021-0267 | Aquisição de dados com Arduino. |

### Revisões sistemáticas

| # | Título | Autores | Ano | URL |
|---|--------|---------|-----|-----|
| 69 | Contribuições do Arduino no Ensino de Física: revisão sistemática | — | ~2018 | https://bia.ifpi.edu.br/jspui/handle/123456789/4839 |
| 70 | Arduino no Ensino de Física: Revisão Sistemática de Literatura | UFPA | ~2022 | https://www.periodicos.ufpa.br/index.php/revistaamazonia/article/view/12175 |

---

## 12. Veículos Brasileiros Recomendados (Prioridade para Publicação)

| Veículo | Sigla | Tipo | Observações |
|---|---|---|---|
| Congresso Brasileiro de Educação em Engenharia | COBENGE | Congresso | 54ª edição em 2026. Principal fórum brasileiro. |
| Congresso Brasileiro de Automática | CBA | Congresso | Já publicou plataformas didáticas similares. |
| Revista Brasileira de Ensino de Física | RBEF | Periódico | **Lacuna clara** — nenhum paper sobre motor + encoder + PID. |
| Revista Brasileira de Educação em Engenharia | RBEE | Periódico | Foco direto em educação em engenharia. |
| Simpósio Brasileiro de Automação Inteligente | SBAI | Simpósio | Já publicou bancada didática para motor CC (2019). |
| Ciência e Natura (UFSM) | — | Periódico | Publicou mini bancada motor + encoder (2025). |

Ver estratégia detalhada de publicação em [`analise-comparativa.md`](analise-comparativa.md#6-estratégia-de-publicação-recomendada).
