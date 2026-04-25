# TCP vs UDP - Comparação Técnica

A diferença entre TCP e UDP está diretamente ligada ao tipo de comunicação e aos requisitos da aplicação. Não existe protocolo "melhor", e sim o mais adequado para cada cenário.

---

## Comparação lado a lado

| Característica        | TCP (Transmission Control Protocol)                         | UDP (User Datagram Protocol)                 |
|----------------------|-------------------------------------------------------------|----------------------------------------------|
| Confiabilidade       | Alta. Garante a entrega dos dados                           | Baixa. Melhor esforço (sem garantia)         |
| Conexão              | Orientado à conexão (3-way handshake)                       | Não orientado à conexão                      |
| Ordem dos Pacotes    | Garantida (reordenação no destino)                          | Não garantida                                |
| Controle de Erro     | Completo (ACK, retransmissão, controle de sequência)        | Básico (checksum)                            |
| Controle de Fluxo    | Sim (janela deslizante)                                     | Não                                          |
| Velocidade           | Mais lento (devido ao controle e validações)                | Mais rápido                                  |
| Overhead             | Alto (cabeçalho mínimo de 20 bytes)                         | Baixo (cabeçalho de 8 bytes)                 |
| Uso comum            | Web, e-mail, transferência de arquivos, APIs                | Streaming, jogos online, VoIP, DNS           |

---

## Funcionamento Técnico

### TCP (Transmission Control Protocol)

O TCP é um protocolo da camada de transporte **orientado à conexão**.

#### Etapas principais:

1. **Estabelecimento de conexão (3-way handshake):**
   - Cliente → Servidor: SYN
   - Servidor → Cliente: SYN + ACK
   - Cliente → Servidor: ACK

2. **Transmissão de dados:**
   - Segmentação dos dados
   - Numeração de sequência
   - Confirmação de recebimento (ACK)

3. **Controle de fluxo e congestionamento:**
   - Janela deslizante (Sliding Window)
   - Ajuste dinâmico da taxa de envio

4. **Encerramento da conexão:**
   - Processo de finalização (FIN/ACK)

#### Características:
- Garante entrega e integridade
- Reenvia pacotes perdidos
- Reordena pacotes automaticamente

---

### UDP (User Datagram Protocol)

O UDP é um protocolo da camada de transporte **sem conexão**.

#### Funcionamento:
- Envia datagramas diretamente, sem estabelecer conexão
- Não há confirmação de entrega (ACK)
- Não há retransmissão automática

#### Características:
- Baixa latência
- Baixo overhead
- Aplicação deve lidar com erros (se necessário)

---

## Quando usar cada um

### TCP (quando confiabilidade é essencial)
- HTTP/HTTPS
- FTP (transferência de arquivos)
- SMTP (e-mail)
- APIs REST

### UDP (quando velocidade é crítica)
- Streaming de vídeo e áudio
- Jogos online
- VoIP (chamadas de voz)
- DNS (consultas rápidas)

---

## Resumo Técnico

- **TCP**: confiável, seguro, porém mais lento
- **UDP**: rápido e leve, porém sem garantias

A escolha depende do trade-off entre **confiabilidade vs latência**.
