Projeto de Fonte de Alimentação Linear Regulada (12V)

Este repositório contém o projeto de uma fonte de alimentação linear regulada, desenvolvida para converter uma tensão alternada (AC) em uma tensão contínua (DC) estável de 12V. O projeto foi integralmente concebido no software Proteus, abrangendo o esquemático elétrico, o layout da placa de circuito impresso (PCB) e a modelagem tridimensional.
Descrição do Circuito

O circuito opera baseado em uma arquitetura linear clássica, dividida em estágios distintos de processamento de energia:

    Retificação: Utiliza uma ponte de diodos (BR1) para realizar a retificação em onda completa da entrada AC proveniente do conector J2.

    Filtragem: O capacitor eletrolítico C3 (1000uF) atua como filtro de ripple, armazenando energia para suavizar a tensão de entrada do regulador.

    Regulação: O circuito integrado LM7812 (U1) garante uma saída estável de 12V DC, compensando variações na tensão de entrada ou na carga conectada.

    Desacoplamento e Sinalização: Os capacitores C2 e C1 (100nF) eliminam ruídos de alta frequência. O LED D1, limitado pelo resistor R1 (100 ohms), indica visualmente o estado de operação do sistema.

Esquemático Elétrico
Desenvolvimento da PCB

O layout da placa de circuito impresso foi desenvolvido focando na integridade das trilhas de alimentação e na dissipação térmica do regulador. O posicionamento dos capacitores de desacoplamento foi otimizado para proximidade com os pinos do CI 7812, garantindo maior eficiência na filtragem.
Layout da Placa
Representação 3D

A visualização tridimensional permite validar o empilhamento dos componentes, a furação dos conectores e o espaço necessário para uma eventual instalação de dissipador de calor no encapsulamento TO-220.
Vista Superior
Vista Inferior
Especificações Técnicas

Componente: U1 | Função: Regulador de Tensão | Valor / Modelo: LM7812
Componente: BR1 | Função: Ponte Retificadora | Valor / Modelo: Bridge (Genérica)
Componente: C3 | Função: Filtro de Ripple | Valor / Modelo: 1000uF / 25V
Componente: C1, C2 | Função: Filtro de Ruído | Valor / Modelo: 100nF (Cerâmico)
Componente: R1 | Função: Resistor de Carga | Valor / Modelo: 100 ohms
Componente: D1 | Função: Indicador de Saída | Valor / Modelo: LED
Notas de Projeto

    Tensão de Entrada: Para assegurar a regulação adequada, a entrada no conector J2 deve resultar em uma tensão mínima de 14.5V DC após a retificação.

    Gestão Térmica: O regulador 7812 dissipa o excesso de tensão em forma de calor. Recomenda-se o uso de dissipador caso a corrente de saída exceda 200mA.

Ferramentas Utilizadas

    Proteus Design Suite (ARES / ISIS)

    Renderizador de PCB 3D
