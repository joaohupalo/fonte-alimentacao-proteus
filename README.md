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
3. **C3 (1000µF)** filtra a ondulação da tensão, suavizando a saída
4. **C2 (100nF)** estabiliza a entrada do regulador
5. O **7812 (U1)** regula a saída para exatamente **12V DC**
6. **C1 (100nF)** estabiliza a saída do regulador
7. O **LED D1** com resistor **R1 (100Ω)** indica que a fonte está energizada
8. A tensão regulada é disponibilizada no conector **J1**

---

## Imagens do Projeto

### Esquemático

<img width="1109" height="289" alt="image" src="https://github.com/user-attachments/assets/933ed0ff-4233-4a9a-b0ee-3483ca06039b" />

---

### Layout PCB

<img width="1194" height="663" alt="image" src="https://github.com/user-attachments/assets/3a4dc8cd-0db9-49a7-ab7e-becff81e7a9f" />

---

### Visualização 3D — Face Superior

<img width="1538" height="841" alt="image" src="https://github.com/user-attachments/assets/5bb7c62f-d2bd-48f5-85a8-798bdeafaf20" />

---

### Visualização 3D — Face Inferior (Trilhas)

<img width="1222" height="613" alt="image" src="https://github.com/user-attachments/assets/8298f688-b205-4e6a-bf32-22c687f9a45a" />

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
│   ├── 01.jpg        # Esquemático do circuito
│   ├── 02.jpg        # Layout da PCB (vista 2D)
│   ├── 03.jpg        # Render 3D - face superior
│   └── 04.jpg        # Render 3D - face inferior (trilhas)
├── proteus/
│   └── CarregadorCelular.pdsprj
└── README.md
```

---

## Licença

Este projeto está sob a licença [MIT](LICENSE).
