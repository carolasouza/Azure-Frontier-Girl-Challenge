# Azure-Frontier-Girl-Challenge

### **Descrição do projeto:**
- Este repositório foi criado para registrar a documentação do desenvolvimento de um agente no Microsoft Azure Foundry.

### **Objetivo do agente:**
- Instructions: "Você é um monitor que auxilia com revisão de questões para o Enem. Suas respostas devem ser limitadas sobre o tema do Enem. Você vai utilizar os arquivos de provas anteriores, contento arquivo de prova e gabaritos, para aplicar questões e corrigir as respostas de quem está interagindo."
- Agent Description: Este agente é um monitor que te auxilia com revisão de questões do Enem.
- Os arquivos das provas utilizado como input de conhecimento estão disponíveis no [link](https://www.gov.br/inep/pt-br/areas-de-atuacao/avaliacao-e-exames-educacionais/enem/provas-e-gabaritos)
<img width="1164" height="593" alt="02 Tela INEP arquivos" src="https://github.com/user-attachments/assets/de0e3248-8323-4358-b821-d56643bafe1d" />

### **Testando o agente:**
- Após fazer as devidas configurações para criação do agente, criando grupo de recurso, recurso do AI Foundry e deploy do modelo de LLM, foram inseridas as instruções, descrição do agente e arquivos de conhecimento.
- Para este agente foi utilizado o gpt-4o-mini
<img width="1289" height="604" alt="01 Instruções e descrição do agente" src="https://github.com/user-attachments/assets/e9bb99dc-3a5e-4fab-a3f0-3dd3b7e3a421" />

- Na tela de inserção de conhecimento, foram carregados os arquivos de apoio e confirmado o carregado
<img width="1110" height="585" alt="03 Tela de carregamento dos arquivos" src="https://github.com/user-attachments/assets/eb0a7c9b-033c-4dfa-a75f-709dfc3379a7" />
<img width="1124" height="599" alt="04 Arquivos carregados" src="https://github.com/user-attachments/assets/8e459eba-7261-4f3d-8d16-c68883ff5fb9" />

- Na primeira interação com o agente, é feita a pergunta "O que você faz?", para validar se as configurações já estão implementadas
<img width="781" height="440" alt="05 Perguntando o que o chat faz" src="https://github.com/user-attachments/assets/f95941ae-4e2a-493e-bcdb-ebc840f71f0d" />

- Em seguida, partimos para a utilização da funcionalidade principal do agente, que é interagir para aprender com questões antigas do ENEM. É solicitada uma pergunta sobre trigonometri, com o seguinte texto: "estou estudando trigonometria, me passe uma questão que já caiu no Enem", com o chat retornando com uma pergunta sobre o tema.
<img width="788" height="406" alt="06 pergunta feita pelo agente" src="https://github.com/user-attachments/assets/66b06244-0c85-4bee-bc37-a4c5e53dfdec" />

- Ao solicitar a data da prova em que a questão foi aplicada, o chat retornou que não é capaz de responder. Fica um ponto de melhoria para a instrução do agente, e verificar se nos arquivos esta informação está disponível.
<img width="1127" height="538" alt="07 solicitando data da prova" src="https://github.com/user-attachments/assets/35045530-1509-49d5-839b-e96fda45a18b" />

- Ao receber a resposta incorreta, o agente apresenta como a questão poderia ser resolvida e faz a devida correção.
<img width="1165" height="655" alt="08 correcao da pergunta" src="https://github.com/user-attachments/assets/fa34ec87-1679-4937-a35d-fe5a5c035cbf" />


### **Referências utilizadas:**
1. Vídeo [Build An AI Agent From Scratch Using Azure AI Foundry](https://youtu.be/wL8H0RySf6I?si=Y1kEpiE0QSLQucCN)
2. [GitHub Miyake-Diogo](https://github.com/Miyake-Diogo/AzureFrontierGirls-AI-Challenge/tree/main)

