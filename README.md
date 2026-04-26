# Curso de Redes de Computadores

<img width="1918" height="1042" alt="Image" src="https://github.com/user-attachments/assets/aea140b4-a6eb-43d1-b28b-c079b6860d3e" />
<img width="1919" height="1079" alt="Image" src="https://github.com/user-attachments/assets/10f15242-2faa-4bc8-bfee-8e8db0327028" />
<img width="1919" height="1073" alt="Image" src="https://github.com/user-attachments/assets/8772a5bd-3659-4e14-bb84-5d5951180e59" />
<img width="1919" height="1075" alt="Image" src="https://github.com/user-attachments/assets/9ef3f643-1583-4c1d-8fed-e33af09ddac4" />
<img width="1913" height="1032" alt="Image" src="https://github.com/user-attachments/assets/66004d4a-c9e3-4ba2-a663-552f5cb01faa" />
<img width="1919" height="1077" alt="Image" src="https://github.com/user-attachments/assets/9fb69e23-597a-4a07-b13a-0b6b2465c6f6" />
<img width="1919" height="1079" alt="Image" src="https://github.com/user-attachments/assets/4632f97d-e966-4c82-a4cd-fcea17fd1089" />
<img width="1919" height="1079" alt="Image" src="https://github.com/user-attachments/assets/e8f51731-800c-40b6-b7bf-1fcd5400fd8a" />

## 📖 Descrição

Este repositório contém meus estudos e práticas sobre **Redes de Computadores**, abordando desde conceitos fundamentais até simulações e configurações práticas de rede.

O objetivo é consolidar conhecimentos essenciais para construção, análise e gerenciamento de redes, com foco em aplicação prática e entendimento técnico.

---

## 🌐 Conceitos Fundamentais

Uma rede de computadores consiste na interconexão entre dispositivos para troca de informações, geralmente no formato de pacotes de dados.

A internet é uma rede global que permite a comunicação entre dispositivos distribuídos mundialmente.

### Modelo em Camadas

A comunicação em rede é organizada em camadas, cada uma com uma função específica:

- Aplicação
- Transporte
- Rede
- Física

### Protocolos de Comunicação

Protocolos são conjuntos de regras que definem como os dados são transmitidos entre dispositivos.

Exemplo:
- TCP (Transporte confiável)
- IP (Endereçamento e roteamento)

---

## 🛠️ Ferramentas e Comandos Utilizados

### Verificação de Conectividade
- `ping` → Testa comunicação entre dispositivos

### Análise de Rotas
- `traceroute` → Mostra o caminho percorrido pelos pacotes

### Consulta DNS
- `nslookup` → Consulta resolução de nomes

---

## 🧪 Simulação e Análise de Rede

### Cisco Packet Tracer

O **Cisco Packet Tracer** é uma ferramenta de simulação de redes que permite criar, configurar e testar ambientes de rede de forma virtual, sem a necessidade de equipamentos físicos.

#### Principais funcionalidades:
- Criação de topologias de rede completas
- Configuração de dispositivos como:
  - Roteadores
  - Switches
  - PCs e servidores
- Simulação de protocolos de rede (TCP/IP, DHCP, DNS)
- Testes de conectividade e fluxo de dados

#### Importância no aprendizado:
O uso do Packet Tracer permite compreender, na prática, como os dispositivos se comunicam, como os pacotes trafegam pela rede e como as configurações impactam diretamente no funcionamento da comunicação.

Além disso, possibilita simular cenários reais, como:
- Redes corporativas
- Segmentação de rede (sub-redes)
- Configuração de serviços (DHCP, DNS, Web)

---

### Wireshark

O **Wireshark** é uma ferramenta avançada de análise de tráfego de rede, utilizada para capturar e inspecionar pacotes de dados em tempo real.

#### Principais funcionalidades:
- Captura de pacotes que trafegam na rede
- Análise detalhada de protocolos (TCP, UDP, HTTP, DNS, etc.)
- Visualização do conteúdo dos pacotes
- Identificação de problemas de rede

#### Importância no aprendizado:
O Wireshark permite entender profundamente o que acontece "por trás" da comunicação entre dispositivos, analisando cada etapa da transmissão de dados.

Com ele é possível:
- Verificar requisições e respostas de rede
- Analisar handshakes do protocolo TCP
- Identificar falhas de comunicação
- Diagnosticar lentidão ou perda de pacotes
- Estudar comportamento de protocolos em diferentes camadas

Essa ferramenta é essencial para desenvolver uma visão mais técnica e detalhada do funcionamento das redes, sendo amplamente utilizada por profissionais de redes e segurança da informação.

---

## 🧪 Práticas Realizadas

- Criação e simulação de redes utilizando o Cisco Packet Tracer
- Implementação de redes com:
  - Hub
  - Switch
  - Roteador
- Conexão de dispositivos com cabos de rede
- Testes de comunicação entre máquinas

---

## 🔄 Dispositivos de Rede

### Hub
- Dispositivo antigo
- Baixa eficiência
- Transmite dados para todos os dispositivos

### Switch
- Mais rápido e seguro
- Direciona dados apenas ao destino correto

### Roteador
- Interliga redes diferentes
- Permite acesso à internet
- Responsável pelo **default gateway**

---

## 🌍 Endereçamento IP

### IPv4
- Formato: 4 octetos (0 a 255)
- Exemplo: `192.168.0.1`
- Classes:
  - A, B, C → Uso geral
  - D → Multicast
  - E → Reservado

### Conceitos importantes
- Máscara de rede
- Sub-redes
- Default Gateway

---

## ⚙️ Configurações de Rede

### DHCP
- Atribuição automática de endereços IP
- Reduz erros de configuração

### DNS
- Tradução de nomes para IP
- Exemplo:
  - `google.com` → IP

---

## 🏢 Intranet

Criação de uma rede interna com:

- Servidor Web
- Servidor DNS
- Compartilhamento de arquivos

### Servidor Web
- Armazena páginas e arquivos
- Acesso via navegador dentro da rede

---

## 📈 Aprendizados

Durante o curso, desenvolvi habilidades importantes como:

- Entendimento das camadas de rede
- Configuração de dispositivos
- Simulação de redes complexas
- Análise de tráfego com ferramentas profissionais
- Organização de redes com sub-redes
- Diagnóstico de problemas de conectividade

---

## 🚀 Objetivo

Construir uma base sólida em redes de computadores, permitindo:

- Criar e gerenciar redes
- Entender comunicação entre dispositivos
- Resolver problemas de rede
- Evoluir para níveis mais avançados

---

## 👨‍💻 Autor

Guilherme Barros
