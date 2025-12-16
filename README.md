# TutorialSistemasComunicaoFPGA
O projeto propõe laboratórios práticos em FPGA para sistemas de comunicação digital, estruturados em blocos funcionais que permitem implementar codificação, modulação e OFDM. Inclui material didático, tutoriais passo a passo para  os experimentos.
## Blocos Implementados

Com base em um levantamento de requisitos e seguindo as especificações, os blocos fundamentais escolhidos para implementação foram:

1.  **Modulação QPSK (Quadrature Phase Shift Keying):**
    * **O que é:** Uma técnica de modulação digital que mapeia pares de bits em símbolos complexos (I+jQ), alterando a fase da portadora para transmitir dois bits por símbolo. É amplamente utilizada em cenários de baixa relação sinal-ruído.
    * **Material Teórico:** [Modulação QPSK e Sua Aplicação](./ARQUIVOS-DIDATICOS/Modulação-QPSK-e-sua-aplicação.pdf)

2.  **Codificação Turbo (Turbo Coding):**
    * **O que é:** Um código corretor de erros (FEC) de alto desempenho, conhecido por sua capacidade de se aproximar do Limite de Shannon. No padrão LTE, é implementado como um PCCC (Parallel Concatenated Convolutional Code) com taxa de 1/3, garantindo robustez contra erros de transmissão.
    * **Material Teórico:** [Codificação Turbo e Sua Aplicação](./ARQUIVOS-DIDATICOS/Codificação-Turbo-e-sua-aplicação.pdf)

3.  **OFDM (Orthogonal Frequency Division Multiplexing):**
    * **O que é:** A base para tecnologias como Wi-Fi, 4G e 5G. É uma técnica de modulação que divide o fluxo de dados em múltiplas subportadoras ortogonais. Isso torna o sistema robusto contra interferência intersimbólica (ISI) causada por multicaminho e permite alta eficiência espectral.
    * **Material Teórico:** [Modulação OFDM e Sua Aplicação](./ARQUIVOS-DIDATICOS/Modulação-OFDM-e-sua-aplicação.pdf)
  
4. **FSK (Frequency Shift Keying):**
   * **O que é:** Uma técnica de modulação digital na qual a informação é transmitida por meio da variação da frequência da portadora. Na forma binária (BFSK), cada bit é representado por uma frequência distinta. Apresenta implementação simples e boa robustez a ruídos, sendo amplamente utilizada em sistemas de comunicação de baixa complexidade e em aplicações didáticas.
   * **Material Teórico:** [Modulação FSK e Sua Aplicação](./ARQUIVOS-DIDATICOS/Modulação%20FSK%20e%20sua%20aplicação.pdf)


## Conteúdo do Repositório



```text
.
├── fsk
│   ├── fsk_digital.qar
│   ├── Modulação FSK e sua aplicação.pdf
│   └── Tutorial FSK.pdf
├── ofdm
│   ├── Modulação OFDM e sua aplicação.pdf
│   ├── ofdm.slx
│   ├── ofdmsystem.qar
│   ├── Tutorial OFDM - Prático.pdf
│   └── Tutorial OFDM - Simulado.pdf
├── qpsk
│   ├── Modulação QPSK e sua aplicação.pdf
│   ├── modulacaoqpsk.slx
│   └── Tutorial QPSK.pdf
├── README.md
└── turbo
    ├── Codificação-Turbo-e-sua-aplicação.pdf
    ├── turbo.slx
    ├── turbo_system.qar
    ├── Tutorial_Pratico.pdf
    └── Tutorial_Simulado.pdf
```

### Tecnologias Utilizadas

* **Modelagem e Simulação:** MATLAB + Simulink
* **Geração de Código:** HDL Coder (do MATLAB)
* **Síntese e Implementação:** Quartus Prime (Intel/Altera FPGA)
* **Verificação de Hardware:** ModelSim

### Passos Principais do Tutorial

1.  **Modelagem em Simulink** 
2.  **Simulação (Simulink)** 
3.  **Geração de VHDL (HDL Coder)** 
4.  **Projeto no Quartus Prime**
5.  **Simulação (ModelSim)**
6.  **Gravação na DE2-115**

## Equipe

* Faber Bernardo Júnior
* Jamilly da Silva Pinheiro
* Jéssica Gomes Carrico

## Licença

Este projeto está licenciado sob a Licença MIT.

Copyright (c) 2025 Faber Bernardo
