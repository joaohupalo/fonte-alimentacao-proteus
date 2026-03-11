# Fonte de Alimentação 12V — Projeto Proteus

Projeto de uma fonte de alimentação regulada de **12V DC** desenvolvido no **Proteus Design Suite**, com esquemático, layout de PCB e visualização 3D.

---

## Descrição

Esta fonte de alimentação converte tensão AC da rede elétrica em **12V DC regulado**, utilizando o regulador linear **7812**. O circuito inclui retificação em ponte, filtragem capacitiva, regulação de tensão e um LED indicador de funcionamento.

---

## Componentes

| Referência | Componente              | Valor / Modelo | Descrição                         |
|------------|-------------------------|----------------|-----------------------------------|
| J2         | Conector de entrada     | SIL-100-02     | Entrada AC (2 pinos)              |
| BR1        | Ponte retificadora      | BRIDGE         | Retificação de onda completa      |
| C3         | Capacitor eletrolítico  | 1000µF         | Filtro de ripple principal        |
| C2         | Capacitor cerâmico      | 100nF          | Desacoplamento na entrada do 7812 |
| U1         | Regulador de tensão     | 7812           | Regulação de saída em 12V         |
| C1         | Capacitor cerâmico      | 100nF          | Desacoplamento na saída do 7812   |
| D1         | LED                     | LED            | Indicador de tensão na saída      |
| R1         | Resistor                | 100Ω           | Limitador de corrente do LED      |
| J1         | Conector de saída       | CONN-SIL2      | Saída DC 12V (2 pinos)            |

---

## Funcionamento

1. A tensão AC entra pelo conector **J2**
2. A **ponte retificadora BR1** converte AC em DC pulsante
3. **C3 (1000µF)** filtra o ripple, suavizando a tensão
4. **C2 (100nF)** estabiliza a entrada do regulador
5. O **7812 (U1)** regula a saída para exatamente **12V DC**
6. **C1 (100nF)** estabiliza a saída do regulador
7. O **LED D1** com resistor **R1 (100Ω)** indica que a fonte está energizada
8. A tensão regulada é disponibilizada no conector **J1**

---

## Imagens do Projeto

### Esquemático

<!-- Adicione aqui a imagem do esquemático -->
> *Substitua pelo caminho da imagem:* `![Esquemático](img/01.png)`

---

### Layout PCB

<!-- Adicione aqui a imagem do layout de PCB -->
> *Substitua pelo caminho da imagem:* `![PCB Layout](img/02.png)`

---

### Visualização 3D — Face Superior

<!-- Adicione aqui a imagem 3D da face superior -->
> *Substitua pelo caminho da imagem:* `![3D - Face Superior](img/03.png)`

---

### Visualização 3D — Face Inferior (Trilhas)

<!-- Adicione aqui a imagem 3D da face inferior -->
> *Substitua pelo caminho da imagem:* `![3D - Face Inferior](img/04.png)`

---

## Dimensões da PCB

| Dimensão | Valor |
|----------|-------|
| Largura  | 80 mm |
| Altura   | 40 mm |

---

## Ferramentas Utilizadas

- **Proteus Design Suite** — Esquemático, PCB e visualização 3D

---

## Estrutura do Repositório

```
/
├── img/
│   ├── 01.png        # Esquemático do circuito
│   ├── 02.png        # Layout da PCB (vista 2D)
│   ├── 03.png        # Render 3D - face superior
│   └── 04.png        # Render 3D - face inferior (trilhas)
├── proteus/
│   └── fonte_12v.pdsprj
└── README.md
```

---

## Licença

Este projeto está sob a licença [MIT](LICENSE).
