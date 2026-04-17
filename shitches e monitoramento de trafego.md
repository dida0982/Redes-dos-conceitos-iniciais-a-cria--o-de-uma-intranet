# Fundamentos de Redes – Análise Técnica

## 1. Switch vs Hub

### Hub
O hub é um dispositivo de camada física (Camada 1 do modelo OSI). Ele opera como um repetidor de sinais, enviando os dados recebidos para **todas as portas**, independentemente do destino.

#### Características:
- Não possui inteligência de encaminhamento
- Opera em broadcast constante
- Alto índice de colisões (CSMA/CD)
- Baixa eficiência e segurança

#### Problemas:
- Compartilhamento de banda
- Vulnerabilidade a sniffing
- Escalabilidade limitada

---

### Switch
O switch opera na Camada 2 (Enlace) do modelo OSI e utiliza endereços MAC para encaminhar quadros de forma inteligente.

#### Funcionamento:
- Mantém uma **tabela MAC (CAM Table)**
- Encaminha quadros apenas para a porta de destino
- Reduz colisões (domínio de colisão isolado por porta)

#### Vantagens:
- Maior desempenho (full-duplex)
- Melhor segurança
- Segmentação de rede eficiente

#### Técnicas utilizadas:
- Frame forwarding
- MAC learning
- VLANs (em switches gerenciáveis)

---

## 2. Wireshark e Análise de Tráfego

O Wireshark é um analisador de protocolos de rede que captura pacotes em tempo real.

### Funcionalidades:
- Captura de pacotes (Packet Sniffing)
- Inspeção profunda (Deep Packet Inspection)
- Filtros de captura e exibição
- Análise de protocolos

### Uso prático:
- Diagnóstico de problemas de rede
- Análise de desempenho
- Identificação de ataques (ex: ARP spoofing, DoS)
- Debug de aplicações que usam rede

### Estrutura de análise:
Cada pacote pode ser analisado em camadas:
- Frame (físico)
- Ethernet (enlace)
- IP (rede)
- TCP/UDP (transporte)
- Aplicação (HTTP, DNS, etc.)

---

## 3. Protocolos e Camadas de Rede (Modelo OSI)

O modelo OSI divide a comunicação em 7 camadas:

1. Física
2. Enlace de Dados
3. Rede
4. Transporte
5. Sessão
6. Apresentação
7. Aplicação

### Importância:
- Padronização da comunicação
- Modularização da rede
- Facilidade de troubleshooting

---

## 4. Protocolo TCP

O TCP (Transmission Control Protocol) atua na Camada 4 (Transporte).

### Características principais:
- Confiável (Reliable)
- Orientado à conexão
- Controle de fluxo
- Controle de congestionamento
- Entrega ordenada

### Funcionamento:

#### 1. Handshake (3-way handshake)
- SYN
- SYN-ACK
- ACK

#### 2. Transmissão de dados
- Segmentação
- Numeração de sequência
- Confirmação (ACK)

#### 3. Encerramento
- FIN / ACK

### Vantagens:
- Garantia de entrega
- Integridade dos dados

### Desvantagem:
- Maior overhead (mais lento que UDP)

---

## 5. Endereçamento IP

O endereço IP identifica um dispositivo na rede.

### IPv4:
- 32 bits
- Exemplo: 192.168.1.1

Dividido em:
- Parte de rede
- Parte de host

---

## 6. Máscara de Rede

A máscara de rede define qual parte do IP pertence à rede e qual ao host.

### Exemplo:
- IP: 192.168.1.10
- Máscara: 255.255.255.0

#### Interpretação:
- Rede: 192.168.1.0
- Host: último octeto

### CIDR:
- Notação simplificada
- Exemplo: /24

---

## 7. Dispositivos na Mesma Rede

Para que dois dispositivos estejam na mesma rede:

### Condição:
- Mesmo endereço de rede após aplicação da máscara

### Exemplo:
- 192.168.1.10/24
- 192.168.1.20/24

→ Estão na mesma rede

---

## 8. Importância na Prática

Dominar esses conceitos permite:

- Configurar redes corretamente
- Evitar conflitos de IP
- Diagnosticar falhas de comunicação
- Melhorar desempenho e segurança
- Projetar redes escaláveis

---

## Conclusão

O entendimento integrado de:
- Dispositivos (switch vs hub)
- Protocolos (TCP/IP)
- Ferramentas (Wireshark)
- Endereçamento (IP + máscara)

é essencial para qualquer profissional de redes, pois permite uma visão completa do funcionamento da comunicação de dados e da infraestrutura de rede.
