```md
# 🌐 Endereçamento IP (IPv4 e IPv6) — Resumo

## 📌 Conceito básico
- Um endereço IP identifica dispositivos em uma rede.
- No **IPv4**, o endereço possui **32 bits**, divididos em **4 octetos** (ex: `192.168.0.1`).
- Cada octeto varia de **0 a 255**.
- Exemplo inválido: `999.0.0.0` ❌

---

## ⚠️ Limites do IPv4
- Mínimo: `0.0.0.0`
- Máximo: `255.255.255.255`
- Não existem valores negativos.

---

## 🌍 Problema do IPv4
- Suporta cerca de **4,3 bilhões de endereços**.
- Isso se tornou insuficiente com o crescimento da internet.

---

## 🚀 IPv6
- Criado para resolver a limitação do IPv4.
- Utiliza **128 bits**.
- Permite cerca de **1 decilhão de endereços**.
- Usa estrutura **hierárquica**.
- Pode funcionar junto com IPv4 via **tunelamento** (encapsulamento).

---

## 🧩 Classes de IP (IPv4)

### 🅰️ Classe A
- Primeiro octeto: **1 a 126**
- Máscara padrão: `255.0.0.0`
- Rede: 1º octeto
- Hosts: 3 últimos octetos
- Exemplo:
  - IP: `123.145.3.3`
  - Rede: `123.0.0.0`
  - Broadcast: `123.255.255.255`

---

### 🅱️ Classe B
- Primeiro octeto: **128 a 191**
- Máscara padrão: `255.255.0.0`
- Rede: 2 primeiros octetos
- Hosts: 2 últimos octetos
- Exemplo:
  - IP: `135.145.3.3`
  - Rede: `135.145.0.0`
  - Broadcast: `135.145.255.255`

---

### 🅲 Classe C
- Primeiro octeto: **192 a 223**
- Máscara padrão: `255.255.255.0`
- Rede: 3 primeiros octetos
- Hosts: último octeto
- Exemplo:
  - IP: `193.168.3.3`
  - Rede: `193.168.3.0`
  - Broadcast: `193.168.3.255`

---

### 🅳 Classe D
- Intervalo: **224 a 239**
- Uso: **Multicast** (comunicação em grupo)

---

### 🅴 Classe E
- Intervalo: **240 a 255**
- Uso: **Pesquisa e testes**

---

## 📡 Conceitos importantes

### 🔹 Endereço de Rede
- Identifica a rede.
- Não pode ser usado por dispositivos.
- Obtido colocando **0 nos bits de host**.

### 🔹 Endereço de Broadcast
- Envia mensagem para todos da rede.
- Obtido colocando **255 nos bits de host**.

---

## 🧠 Comparação geral

| Característica | IPv4 | IPv6 |
|------|------|------|
| Bits | 32 | 128 |
| Endereços | ~4,3 bilhões | ~1 decilhão |
| Formato | Decimal | Hexadecimal |
| Situação | Ainda usado | Substituto |

---

## 📍 Observação final
- Nem todo IP é público.
- Existem **IPs privados**, usados dentro de redes locais.
```
