# 🖼️ Impressões de Execução

Este documento reúne as evidências visuais (prints) da execução do projeto **Sistema de Classificação de Dados com RBAC**.  
Cada print está acompanhado do comando utilizado e da explicação correspondente.

---

## 1️⃣ Classificação e Risco dos Arquivos (Diretor)

📷 Evidência:  
![Diretor](evidencias/print1.png)

🔹 Comando usado:
python3 main.py

🔹 Explicação:
Executa o programa principal com papel Diretor, permitindo acesso a todos os arquivos.
O sistema exibe a classificação e o risco de cada documento e gera o relatório de risco.

---

## 2️⃣ Auditoria de Acessos Negados (Analista)

📷 Evidência:  
![Analista](evidencias/print2.png)

🔹 Comando usado:
cat reports/audit.log

🔹 Explicação:
Exibe o conteúdo do arquivo de auditoria (audit.log).
Mostra as tentativas de acesso negadas para o papel Analista, incluindo horário, papel e documento acessado.

---

## 3️⃣ Classificação e Risco dos Arquivos (Estagiário)

📷 Evidência:  
![Estagiário](evidencias/print3.png)

🔹 Comando usado:
python3 main.py

🔹 Explicação:
Executa o programa principal com papel Estagiário.
Nesse caso, o sistema nega acesso aos arquivos conforme as regras de RBAC, registrando os eventos no log de auditoria.

---

## 4️⃣ Relatório de Risco

📷 Evidência:  
![Relatório](evidencias/print4.png)

🔹 Comando usado:
cat reports/relatorio_risco.txt

🔹 Explicação:
Exibe o relatório de risco gerado pelo sistema.
Lista os documentos classificados e seus respectivos níveis de risco, servindo como base para compliance e acompanhamento.

---

## 5️⃣ Auditoria Completa

📷 Evidência:  
![Auditoria](evidencias/print5.png)

🔹 Comando usado:
cat reports/audit.log

🔹 Explicação:
Mostra o log completo de auditoria, incluindo todas as tentativas de acesso (permitidas e negadas).
É útil para monitoramento, rastreabilidade e análise de comportamento de usuários.

---

## ✅ Evidências Comprovadas

✔ Classificação automática de documentos  
✔ Avaliação de risco  
✔ Controle de acesso baseado em papéis (RBAC)  
✔ Auditoria e geração de relatórios  
✔ Estrutura organizada para governança de dados
