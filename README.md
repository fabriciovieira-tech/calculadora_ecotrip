# Projeto EcoTrip: Simulador de Impacto Ambiental

O **EcoTrip** é um simulador projetado para conscientizar usuários sobre o impacto ambiental de seus deslocamentos, calculando a emissão de gases de efeito estufa com base na distância percorrida e no modal de transporte escolhido.

---

## 🛠️ Especificações Técnicas

*   **Design:** UI/UX desenvolvido no **Figma**, com foco em usabilidade e estética moderna.
*   **Frontend:** Estruturado em **HTML5** e estilizado com **CSS3** (utilizando conceitos de cards, sombras suaves e tipografia limpa).
*   **Backend & Lógica:** Implementado em **JavaScript (ES6)**, utilizando `localStorage` para a persistência de dados entre páginas de forma eficiente.

---

## 📐 Estrutura do Sistema

### 1. Interface de Entrada (`index.html`)
A página principal apresenta um formulário intuitivo para coleta de dados:
*   **Campos de Entrada:** Origem, Destino e Distância (em km).
*   **Seleção de Veículo:** Substituímos menus convencionais por **cards interativos** com ícones (Carro, Moto, Ônibus e Caminhão) que mudam de estado visual ao serem selecionados, reforçando a experiência do usuário (UX).

### 2. Processamento e Resultados (`resultado.html`)
Esta página recupera os dados inseridos, aplica a lógica de cálculo e exibe o impacto ambiental de forma contextualizada.

#### Fatores de Emissão Utilizados:
O sistema utiliza coeficientes específicos para calcular a liberação de CO₂ por quilômetro:

| Veículo | Emissão (kg de CO₂ por km) |
| :--- | :--- |
| **Moto** | 0.05 kg |
| **Carro** | 0.12 kg |
| **Ônibus** | 0.80 kg |
| **Caminhão** | 1.20 kg |

---

## 💡 Diferenciais do Projeto

*   **Fidelidade ao Design:** Tradução fiel dos protótipos do Figma para o código real, garantindo uma interface moderna e limpa.
*   **Lógica Dinâmica:** O JavaScript aplica um "fator de poluição" variável de acordo com o modal escolhido, garantindo precisão na simulação.
*   **Feedback Contextual:** A página de resultados exibe mensagens personalizadas, permitindo que o usuário compreenda a magnitude da sua pegada de carbono conforme o veículo utilizado.