<div align="center">
  <img src="src/logo-phishio.png" alt="Logo Phishio" width="120" />
  
  # 🛡️ Phishio
  
  **Site Oficial da Extensão**
  
  <p><em>Este é um repositório exclusivamente destinado para alocar o site oficial (Landing Page) da extensão Phishio.</em></p>
</div>

---

## 📖 Sobre o Phishio
O Phishio é um sistema híbrido para detecção de phishing em tempo real, desenvolvido como um Trabalho de Conclusão de Curso (TCC). 

O projeto utiliza uma abordagem dupla que combina a precisão da **Recuperação de Informação** (utilizando o Modelo Vetorial e cálculos de TF-IDF) com o poder do **Crowdsourcing** para a validação comunitária de URLs suspeitas.

## 🏗️ Arquitetura do Sistema
A arquitetura completa do projeto é dividida em dois componentes principais:

### ⚙️ 1. API Backend
* **Desenvolvimento:** Construída em `Python` utilizando o framework `FastAPI`.
* **Motor Vetorial:** Responsável pela análise profunda de conteúdo das páginas utilizando cálculos de **TF-IDF**.
* **Banco de Dados:** Gerenciamento da reputação das URLs e dos votos da comunidade integrado diretamente ao **Firebase (Firestore)**.

### 🧩 2. Extensão para Google Chrome
* **Tecnologia:** Construída sob as diretrizes modernas do **Manifest V3**.
* **Atuação:** Opera como o cliente do sistema, analisando as páginas visitadas pelo usuário de forma otimizada.
* **Feedback Visual:** Fornece retorno em tempo real através de um Popup interativo guiado por estados claros:
  * 🟢 Seguro
  * 🟡 Suspeito
  * 🔴 Perigoso
* **Interatividade:** Alerta o usuário oferecendo ações seguras para evitar o roubo de dados. Além disso, a interface permite reportar sites maliciosos facilmente, alimentando diretamente a base de dados de Crowdsourcing.

---

## 👨‍💻 Desenvolvedores
* **Lucas dos Santos Lima**
* **Pedro Henrique Gomes Lückeroth**

*Trabalho de Conclusão de Curso - PUC Minas*