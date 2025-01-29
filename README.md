# Azure Machine Learning - Previsão de Aluguéis de Bicicletas  

##  O que é o Microsoft Azure?  
O **Microsoft Azure** é uma plataforma de computação em nuvem que oferece diversos serviços para desenvolvimento, armazenamento, análise de dados, inteligência artificial, aprendizado de máquina e muito mais. Ele permite que desenvolvedores e empresas criem, implantem e gerenciem aplicativos e modelos de machine learning em um ambiente seguro, escalável e globalmente disponível.  

---

##  Sobre o Projeto  
Neste projeto, foi criado um **modelo de aprendizado de máquina automatizado** para prever o número de bicicletas alugadas com base em diferentes variáveis. O modelo foi desenvolvido no **Azure Machine Learning** utilizando técnicas de regressão.  

---

##  Passo a Passo: Criando o Serviço de Machine Learning no Azure  

### 1️⃣ Criar um Recurso no Azure  
1. Acesse o portal do Azure: **[https://portal.azure.com](https://portal.azure.com)**
2. No menu, clique em **"Criar um recurso"**.
3. Selecione **"Azure Machine Learning"**.
4. Preencha as configurações iniciais, incluindo:
   - **Básico (Basics)**: Nome do serviço, região, grupo de recursos.
   - **Rede (Networking)**: Configurações de acesso.
   - **Criptografia (Encryption)**: Método de segurança para dados.
   - **Identidade (Identity)**: Permissões de autenticação.
   - **Tags**: Informações adicionais para organização.
5. Clique em **"Revisar + Criar"** e aguarde a validação das informações.
6. Após a validação, clique em **"Criar"** para provisionar o serviço.  

---

### 2️⃣ Acessar o Azure Machine Learning  
1. Acesse o portal do Azure Machine Learning: **[https://ml.azure.com](https://ml.azure.com)**.  
2. Selecione o workspace criado na etapa anterior.  
3. No menu lateral, clique em **"Automated ML"** para iniciar um novo projeto de Machine Learning Automatizado.  

---

### 3️⃣ Configuração do Projeto de Machine Learning  
1. Clique em **"Novo experimento"** e configure:  
   - **Nome do experimento**: Define um nome descritivo.  
   - **Descrição**: Informa o objetivo do modelo.  
   - **Tipo de Tarefa**: Selecionei como **Regressão** (pois queremos prever valores numéricos).  

2. Configure o ativo de dados:  
   - **Nome e descrição** do dataset.  
   - **Fonte dos dados**: Foi utilizado o dataset disponível em **[https://aka.ms/bike-rentals](https://aka.ms/bike-rentals)**.  
   - **Esquema e tipo dos dados**: Define corretamente os tipos de cada coluna.  

---

### 4️⃣ Configuração das Tarefas de Treinamento  
1. **Coluna de destino**: Seleciona a variável **rentals (integer)** como alvo da previsão.  
2. **Modelos permitidos**: Foram utilizados **RandomForest** e **LightGBM**.  
3. **Limites e Validação**: Configura parâmetros como número máximo de iterações e método de validação cruzada.  
4. **Configuração de Computação**: Escolhe uma máquina virtual adequada para treinar o modelo.  

---

### 5️⃣ Treinamento e Validação  
1. Após definir as configurações, inicie o treinamento.  
2. Monitore o progresso na aba **"Tarefas (Jobs)"** dentro do portal do Azure Machine Learning.  
3. Após a conclusão, analise os resultados e escolha o melhor modelo com base nas métricas apresentadas.  

---

## 📂 Métricas 
![image](https://github.com/user-attachments/assets/e57fb9d4-72eb-487d-a1ca-b89551f9fc0c)
![image](https://github.com/user-attachments/assets/a83d7de2-5aaa-4377-bccf-04f385671e5d)
![image](https://github.com/user-attachments/assets/6ef8d19b-b534-471e-b75d-3a50ae1a3fb9)
![image](https://github.com/user-attachments/assets/a58f8552-df70-4dc2-bd1c-a471814c7082)




---
