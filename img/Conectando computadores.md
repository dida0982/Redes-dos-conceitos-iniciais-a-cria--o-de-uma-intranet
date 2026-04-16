# Fundamentos de Redes - Explicação Técnica

## 1. Cisco Packet Tracer

O Cisco Packet Tracer é um simulador de redes utilizado para modelar, configurar e testar topologias de rede sem a necessidade de hardware físico.

### Funcionamento técnico:
- Permite a criação de topologias (estrela, barramento, malha, etc.)
- Simula dispositivos de rede:
  - Hosts (PCs)
  - Switches (Camada 2)
  - Roteadores (Camada 3)
- Configuração de:
  - Endereçamento IP (IPv4/IPv6)
  - Máscara de sub-rede
  - Gateway padrão

### Simulação:
- Encapsulamento de dados (Modelo OSI/TCP-IP)
- Comunicação entre dispositivos
- Execução de protocolos como:
  - ARP
  - ICMP
  - DNS

---

## 2. Rede com Hub

O hub é um dispositivo que opera na Camada 1 (Física) do modelo OSI.

### Funcionamento técnico:
- Não interpreta dados, apenas sinais elétricos
- Ao receber um frame em uma porta:
  - Replica para todas as outras portas
- Não possui:
  - Tabela MAC
  - Inteligência de encaminhamento

### Consequências:
- Um único domínio de colisão
- Uso do protocolo CSMA/CD
- Baixa eficiência da rede

### Testes:
- Uso do comando `ping`
- Verificação da comunicação entre hosts

---

## 3. Comando nslookup

O comando `nslookup` é utilizado para consultar servidores DNS e resolver nomes de domínio.

### Funcionamento técnico:
1. O usuário executa:
```

nslookup google.com

```
2. O sistema consulta um servidor DNS
3. O DNS retorna:
- Endereço IP (registro A)
- Outros registros (MX, CNAME, etc.)

### Exemplo de saída:
```

Server:  8.8.8.8
Name:    google.com
Address: 142.250.x.x

```

### Conceitos envolvidos:
- Porta 53 (UDP/TCP)
- Resolução recursiva e iterativa
- Cache DNS
- Hierarquia DNS:
  - Root
  - TLD
  - Servidores autoritativos

---

## 4. Conexão com Cabos

A conexão entre dispositivos segue padrões de cabeamento estruturado.

### Tipos de cabos:

#### Cabo direto (straight-through)
- Usado entre dispositivos diferentes:
  - PC → Switch
  - Switch → Roteador
- Mesmo padrão nas duas pontas (568A ou 568B)

#### Cabo cruzado (crossover)
- Usado entre dispositivos iguais:
  - PC → PC
  - Switch → Switch (antigo)
- Troca dos pares TX e RX

#### Auto MDI/MDIX
- Dispositivos modernos detectam automaticamente o tipo de cabo

### Camada envolvida:
- Camada 1 (Física)
- Transmissão de bits via sinais elétricos

---

## Visão Geral (Modelo OSI)

- Camada 1 (Física): Cabos e Hub
- Camada 2 (Enlace): Frames e comunicação local
- Camada 3 (Rede): Endereçamento IP
- Camada 7 (Aplicação): DNS (`nslookup`)
```
