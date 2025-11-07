# Sprint-4----Edge-Computing-

⚽ Sistema de Registro e Pontuação de Jogadoras com LCD I2C
🧩 Projeto desenvolvido para a disciplina Edge Computing - FIAP
👥 Equipe
Nome	RM
Athur Alberini Soares Pereira	565954
Fabio Pereira Rogério Júnior	564005
Kauã Veloso Lima	561954
Matheus Tonsa Martini	564454
Sebastian Iriarte Gonzales	563619
📖 Sobre o Projeto

Este projeto tem como objetivo simular um sistema interativo de registro e pontuação de jogadoras de futebol, utilizando um display LCD I2C (20x4) e botões físicos conectados a um ESP32.

O sistema permite:

Registrar gols e assistências por jogadora;

Exibir o placar geral atualizado;

Calcular automaticamente a “Craque da Partida”, com base em uma pontuação de desempenho.

A implementação foi realizada no simulador Wokwi, utilizando a linguagem C++ (Arduino).

⚙️ Arquitetura e Funcionamento
🧠 Estrutura Lógica

O sistema é composto por três modos principais de operação:

Registro de Jogadoras
→ Permite selecionar uma jogadora e registrar um gol ou uma assistência.

Placar Geral
→ Mostra as estatísticas completas de todas as jogadoras, com rolagem automática no LCD.

Craque da Partida
→ Calcula automaticamente a jogadora destaque com base na fórmula:

Pontuação = (Gols × 2) + Assistências

🔌 Componentes Utilizados
Componente	Função
ESP32 DevKit v1	Microcontrolador principal
LCD 20x4 I2C (endereço 0x27)	Exibição de informações
4 Botões tácteis	Navegação e controle
Jumpers	Conexões entre componentes
🕹️ Interação com o Usuário
Botão	Cor	Função
BTN_UP	🟢 Verde	Navegar para cima
BTN_DOWN	🔵 Azul	Navegar para baixo
BTN_SELECT	🔴 Vermelho	Confirmar seleção
BTN_MENU	🟡 Amarelo	Alternar telas / Resetar estatísticas (pressão longa)

Todos os botões utilizam INPUT_PULLUP, ou seja, permanecem em estado HIGH e são ativados ao serem pressionados (LOW).

🖥️ Telas do Sistema
🔸 Tela 1 — Seleção de Jogadora

Permite escolher a jogadora ativa:

SELECIONE A JOGADORA
>MARTA
 MANUELA
 JULIA

🔸 Tela 2 — Registro de Ação

Após selecionar a jogadora, é possível registrar Gol ou Assistência.

🔸 Tela 3 — Placar Geral

Mostra as estatísticas completas:

MARTA   G:2  A:1
MANUELA G:1  A:0
JULIA   G:0  A:3

🔸 Tela 4 — Craque da Partida

Exibe a jogadora com maior pontuação:

CRAQUE DA PARTIDA:
>MARTA (5 pts)

🧰 Tecnologias e Bibliotecas
Tecnologia	Descrição
C++ / Arduino	Linguagem de programação
ESP32 DevKit	Plataforma de desenvolvimento
Wire.h	Comunicação I2C
LiquidCrystal_I2C.h	Controle do display LCD
💻 Simulação no Wokwi

🔗 Acesse o projeto completo:
👉 https://wokwi.com/projects/442258934652584961

📸 Captura da Simulação

🚀 Melhorias Futuras

💾 Armazenar estatísticas em EEPROM ou SPIFFS para persistência de dados.

🧑‍💻 Adicionar modo de configuração para cadastro de novas jogadoras.

🖤 Atualizar interface para display OLED com ícones gráficos.

🏅 Implementar ranking acumulado entre partidas.

🧾 Licença

Este projeto foi desenvolvido para fins educacionais, como parte da disciplina Edge Computing no curso de Engenharia de Software - FIAP.
O código é de uso livre para fins acadêmicos, desde que mantida a citação da equipe desenvolvedora.

🏁 Créditos Finais

“A tecnologia é uma ferramenta poderosa quando usada para promover o esporte, a competição e o aprendizado.”
— Equipe FIAP ⚙️

✨ Desenvolvido com dedicação, criatividade e trabalho em equipe.
