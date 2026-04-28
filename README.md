#Phishio
Este é um Repositório exclusivamente para alocar o site da extensão Phishio.

Sobre
Phishio é um sistema híbrido para detecção de phishing em tempo real, desenvolvido como um Trabalho de Conclusão de Curso (TCC).

O projeto utiliza uma abordagem dupla que combina Recuperação de Informação (com Modelo Vetorial e TF-IDF) e Crowdsourcing para a validação de URLs suspeitas.

Arquitetura
A arquitetura é composta por dois componentes principais:

API Backend: Desenvolvida em Python com FastAPI, responsável pela análise de conteúdo (motor vetorial TF-IDF) e gerenciamento da reputação de URLs (via Firestore).
Extensão para Google Chrome: Atua como cliente (compatível com Manifest V3), analisando as páginas visitadas. Ela fornece feedback visual em tempo real através de um Popup interativo guiado por estados (seguro, suspeito, perigoso) e alerta o usuário oferecendo ações seguras. A interface também permite que o usuário reporte sites, alimentando diretamente a base de Crowdsourcing.