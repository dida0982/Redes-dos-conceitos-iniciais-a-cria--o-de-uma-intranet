# Configuração de Rede: DHCP, Intranet, Servidores Web e DNS

## 1. Atribuição Automática de IP com DHCP

O **DHCP (Dynamic Host Configuration Protocol)** é um protocolo responsável por automatizar a configuração de rede dos dispositivos.

### Funcionamento:
- O cliente envia uma requisição (DHCP Discover) na rede.
- O servidor DHCP responde com uma oferta de IP (DHCP Offer).
- O cliente solicita o IP ofertado (DHCP Request).
- O servidor confirma a atribuição (DHCP Acknowledgment).

### Vantagens:
- Elimina configuração manual de IP.
- Reduz erros de configuração.
- Facilita gerenciamento de redes grandes.

---

## 2. Construção de uma Intranet com Servidores

Uma **intranet** é uma rede privada utilizada dentro de uma organização.

### Componentes principais:
- Servidor de arquivos
- Servidor web
- Servidor DNS
- Switches e roteadores
- Clientes (computadores/dispositivos)

### Características:
- Acesso restrito (interno)
- Alta segurança
- Compartilhamento de recursos

---

## 3. Configuração de Servidor Web na Intranet

O servidor web permite hospedar páginas e arquivos acessíveis dentro da rede interna.

### Etapas básicas:
1. Instalar um servidor web (ex: Apache, Nginx).
2. Configurar diretório raiz (onde os arquivos ficam armazenados).
3. Definir permissões de acesso.
4. Testar acesso via navegador usando o IP do servidor.

### Exemplo de acesso:
http://192.168.0.10


### Funcionalidades:
- Hospedagem de sites internos
- Compartilhamento de documentos
- Sistemas corporativos

---

## 4. Configuração de Servidor DNS

O **DNS (Domain Name System)** traduz nomes de domínio em endereços IP.

### Objetivo:
Permitir que usuários acessem serviços usando nomes amigáveis em vez de IPs.

### Exemplo:
intranet.local → 192.168.0.10


### Etapas básicas:
1. Instalar servidor DNS (ex: BIND, Windows DNS).
2. Criar zona de domínio (ex: intranet.local).
3. Adicionar registros DNS:
   - Tipo A (nome → IP)
4. Configurar clientes para usar o servidor DNS.

### Vantagens:
- Facilidade de acesso
- Melhor usabilidade
- Abstração de endereços IP

---

## Conclusão

A integração entre DHCP, servidores web e DNS dentro de uma intranet permite:

- Automatização da rede
- Organização dos serviços internos
- Facilidade de acesso e gerenciamento
- Maior eficiência operacional
