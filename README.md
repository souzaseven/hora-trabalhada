# ⏱️ Calculadora de Horas Trabalhadas

Uma ferramenta web para calcular horas trabalhadas, intervalos e horas extras com precisão.
<!--
![Preview da Calculadora](https://raw.githubusercontent.com/souzaseven/Site2/Desafios/icon%20eu.ico)
-->
## ✨ Funcionalidades

- **Cálculo Completo**:
  - Horas do primeiro turno
  - Horas do segundo turno
  - Duração do intervalo
  - Total de horas trabalhadas
  - Cálculo automático de horas extras

- **Recursos Inteligentes**:
  - Navegação automática entre campos
  - Cálculo em tempo real
  - Formatação clara dos resultados
  - Detecção de horas extras (>8h)

- **Design Moderno**:
  - Interface limpa e intuitiva
  - Responsivo para todos dispositivos
  - Cores temáticas azuis

## 🛠️ Tecnologias Utilizadas

- **Frontend**:
  - HTML5 semântico
  - CSS3 moderno
  - JavaScript puro (ES6+)

- **Bibliotecas**:
  - Font Awesome (ícones)
  - Google Analytics (métricas)
  - Google AdSense (monetização)

## 📂 Estrutura de Arquivos
calculadora-horas/ <br>
├── index.html # Página principal <br>
├── style.css # Estilos personalizados <br>
└── script.js # Lógica da calculadora <br>


## ⚙️ Como Funciona

### Cálculo Principal
```javascript
function calcularHorasTrabalhadas() {
    const start1 = new Date(`01/01/2000 ${startTime1}`);
    const end1 = new Date(`01/01/2000 ${endTime1}`);
    const diffTurno1 = (end1 - start1) / (1000 * 60);
    
    // Cálculos similares para turno2 e intervalo
    // ...
    
    const horasTrabalhadas = Math.floor(totalMinutosTrabalhados / 60);
    const minutosTrabalhadas = totalMinutosTrabalhados % 60;
    
    document.getElementById('result').innerText = 
        `Total de horas trabalhadas: ${horasTrabalhadas}h ${minutosTrabalhadas}min`;
}
```

Navegação Automática
function verificarProximoCampo(campoAtual, proximoCampo) {
    if (document.getElementById(campoAtual).value.length === 5) {
        document.getElementById(proximoCampo).focus();
    }
    calcularHorasTrabalhadas();
}


Detecção de Horas Extras
if (horasTrabalhadas > 8) {
    const minutosExtras = (horasTrabalhadas - 8) * 60 + minutosTrabalhadas;
    // Exibe horas extras formatadas
}

🎨 Design
Tema Azul Moderno:
Fundo azul (#007ced)
Card branco com sombras
Bordas e destaques em azul

Elementos UI:
Campos de tempo espaçados
Botão de limpar vermelho
Ícones intuitivos
Tipografia clara

💡 Dicas de Uso
Para calcular:
Preencha os horários de entrada/saída
Os cálculos são automáticos
Foque no próximo campo automaticamente

Personalização:
/* Alterar cores principais */
.calculator {
    background-color: #f5f5f5;
    border: 2px solid #3f51b5;
}

.calculator h1 {
    color: #3f51b5;
    border-bottom-color: #3f51b5;
}

