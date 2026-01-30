🎮 Calculadora de Partidas Rankeadas
Um sistema simples para calcular o nível de jogadores em jogos competitivos baseado no saldo de vitórias.

🚀 Funcionalidades

✅ Calcula saldo (vitórias - derrotas)

✅ Determina nível conforme tabela oficial

✅ Interface simples e intuitiva

✅ Validação de entrada

✅ Código modular e reutilizável

📊 Tabela de Níveis
Saldo Vitórias	Nível
≤ 10	Ferro
11-20	Bronze
21-50	Prata
51-80	Ouro
81-90	Diamante
91-100	Lendário
≥ 101	Imortal

📁 Estrutura

text
calculadora-ranqueada/
├── index.js          # Código principal
├── README.md         # Documentação
└── package.json      # Configurações (opcional)


💻 Como Usar

Versão Terminal (Node.js)
bash
git clone https://github.com/seu-usuario/calculadora-ranqueada.git
cd calculadora-ranqueada
node index.js
Versão Web
Copie o código para o console do navegador ou crie um arquivo HTML.

📝 Código Principal

javascript

function calcularNivel(vitorias, derrotas) {
    const saldo = vitorias - derrotas;
    let nivel;
    
    if (saldo <= 10) nivel = "Ferro";
    else if (saldo <= 20) nivel = "Bronze";
    else if (saldo <= 50) nivel = "Prata";
    else if (saldo <= 80) nivel = "Ouro";
    else if (saldo <= 90) nivel = "Diamante";
    else if (saldo <= 100) nivel = "Lendário";
    else nivel = "Imortal";
    
    return `O Herói tem saldo de ${saldo} e está no nível ${nivel}`;
}

// Exemplo de uso
console.log(calcularNivel(75, 20)); // Saldo: 55 → Ouro
🧪 Exemplos
javascript
calcularNivel(5, 5)    // "Ferro"
calcularNivel(15, 3)   // "Bronze" 
calcularNivel(40, 10)  // "Prata"
calcularNivel(120, 20) // "Imortal"


🛠 Tecnologias

- JavaScript ES6+
- Node.js (opcional)
- Git para versionamento

📈 Próximos Passos
Interface web com HTML/CSS

Banco de dados para histórico

API REST para integração

Sistema multiplayer

🤝 Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests.

Desenvolvido como projeto prático do bootcamp DIO
