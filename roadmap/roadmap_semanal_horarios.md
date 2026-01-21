# 🔐 Roadmap SOC Analyst → Pentester Junior
## Calendário Diário de Estudo Completo (26 Semanas)

**Duração:** 6 Meses (17 Jan - 17 Jul 2026)  
**Intensidade:** 3h30min/dia (210 min)  
**Foco:** SOC Analyst → Pentester Junior (Network Analysis + Wireshark)

---

## 📋 Resumo Executivo

| Aspecto | Detalhes |
|---------|----------|
| **Período** | 17 de Janeiro - 17 de Julho de 2026 (6 meses) |
| **Tempo Diário** | 210 minutos (3h30min) - Dias completos |
| **Dias Leves** | Ter/Qui = 160 min \| Sáb = 150 min \| Dom = 60 min (opcional) |
| **Total de Horas** | ~560 horas reais de estudo em 26 semanas |
| **Estrutura** | PRÉ-ROADMAP + 4 FASES |

---

## ⏰ Estrutura de Tempo Diária

### Dias Completos (Seg/Qua/Sex = 210 min)

| Horário | Duração | Atividade |
|---------|---------|-----------|
| 08:00-09:00 | 60 min | Tópico Principal - TEORIA |
| 09:00-10:00 | 60 min | Tópico Principal - PRÁTICA/LAB |
| 10:00-10:45 | 45 min | Tópico Secundário - PRÁTICA |
| 10:45-11:15 | 30 min | Consolidação + Revisão (notas) |
| 11:15-11:50 | 35 min | Projetos + Publicação (GitHub/Blog) |

### Dias Leves (Ter/Qui = 160 min)

| Horário | Duração | Atividade |
|---------|---------|-----------|
| 08:00-09:00 | 60 min | Tópico Principal - Continuação |
| 09:00-10:00 | 60 min | Prática/Lab do dia |
| 10:00-10:30 | 30 min | Livro + Wireshark (revisão) |
| 10:30-11:00 | 30 min | Revisão Geral |

---

# FASE 0: PRÉ-ROADMAP (Semana 0 - 17-21 Jan 2026)

## Objetivo
Estabelecer fundações sólidas em computação básica antes de começar oficialmente.

> **Importante:** Se você já conhece estes tópicos, **pule para a Fase 1**. Senão, dedique 3-5 dias aqui.

### SEGUNDA (17 Jan) - Como o Computador Funciona

**Teoria (60 min):**
- CPU, GPU, RAM, HD/SSD - Arquitetura Von Neumann
- Fetch-decode-execute cycle
- Clock/GHz em processadores

**Prática (60 min):**
- Abrir Task Manager (Windows) ou `top` (Linux)
- Ver processos em tempo real
- Notar CPU, memória, disco

**Consolidação (30 min):**
- Desenhar diagrama componentes no papel

### TERÇA (18 Jan) - Sistema Binário

**Teoria (60 min):**
- Bits, bytes, conversão decimal-binário
- Por que tudo é 1s e 0s
- Exemplo: 5 em decimal = 101 em binário

**Prática (60 min):**
```bash
python3
>>> bin(5)
'0b101'
>>> int('101', 2)
5
```

**Revisão (30 min):**
- Entender permissões Linux (755 em binário = 111 101 101)

### QUARTA (19 Jan) - Software vs Hardware

**Teoria (60 min):**
- Diferenças entre hardware (físico) e software (programas)
- SO como intermediário
- Exemplos práticos

**Prática (60 min):**
```bash
uname -a
cat /proc/cpuinfo
lsb_release -a
```

**Consolidação (30 min):**
- Notas em Obsidian

### QUINTA (20 Jan) - Sistema Operacional Básico

**Teoria (60 min):**
- Processos, threads, memory management
- Permissões de arquivo
- Como SO controla recursos

**Prática (60 min):**
```bash
ps aux
top
chmod 755 arquivo
ls -l
```

**Revisão (30 min):**
- Resumo de tudo em uma página

### SEXTA (21 Jan) - Arquiteturas x86/x64/ARM

**Teoria (60 min):**
- 32-bit vs 64-bit
- ARM para mobile/IoT
- Por que exploits precisam ser arquitetura correta

**Prática (60 min):**
```bash
uname -m
getconf LONG_BIT
file /bin/bash
```

**Consolidação (30 min):**
- Criar arquivo `PRE-ROADMAP.md` no GitHub

---

# FASE 1: FUNDAÇÕES SÓLIDAS (Semanas 1-6: 24 Jan - 6 Mar 2026)

## Objetivo
Dominar Linux, Python básico, redes TCP/IP e Wireshark. Tudo que você precisa para não se perder depois.

---

## Semana 1 (24-30 Jan): Linux Parte 1 + Intro TCP/IP

### SEGUNDA (24 Jan) - Linux: Estrutura de Diretórios e Comandos Básicos

**Tópico Principal:** Linux Filesystem + Comandos Core

**08:00-09:00 (Teoria):**
- Estrutura de diretórios: `/`, `/home`, `/etc`, `/var`, `/bin`, `/usr`
- Por que cada pasta existe
- Comando: `man hier`

**09:00-10:00 (Prática):**
```bash
pwd                          # onde está
ls -la                       # listar com detalhes
cd /etc                      # mudar pasta
mkdir -p ~/roadmap/{linux,python,networks}
ls -la /
file /bin/bash
```

**10:00-10:45 (Tópico Secundário - Python):**
- Instalação Python (WSL se Windows)
- `python3 --version`
- Primeiro script: `print("Hello, Security!")`

**10:45-11:15 (Consolidação):**
- Criar arquivo: `~/roadmap/Linux_Week1.md`
- Listar comandos do dia com explicações
- Screenshot: estrutura criada

**11:15-11:50 (GitHub):**
```bash
git init roadmap-seg-2026
cd roadmap-seg-2026
git add .
git commit -m "add: week 1 - linux basics"
git push
```

### TERÇA (25 Jan) - Linux: Permissões e Ownership

**08:00-09:00 (Teoria):**
- Permissões: rwx (read/write/execute)
- Octal: 755 (rwx r-x r-x), 644 (rw- r-- r--)
- SUID, SGID, sticky bit
- Por que SUID é security risk

**09:00-10:00 (Prática):**
```bash
touch arquivo.txt
ls -l arquivo.txt                    # ver permissões atuais
chmod 644 arquivo.txt               # rw-r--r--
chmod 755 script.sh                 # rwxr-xr-x
chmod 4755 programa                 # SUID (danger!)
ls -l script.sh
```

**10:00-10:30 (Revisão):**
- Tabela conversão octal-rwx em anotações

**10:30-11:00 (Revisão):**
- Entender riscos SUID em segurança

### QUARTA (26 Jan) - Linux: Gerenciamento de Processos e Logs

**08:00-09:00 (Teoria):**
- Processos, PIDs, sinais (SIGTERM, SIGKILL)
- `ps`, `top`, `kill`
- Diferença entre signals

**09:00-10:00 (Prática):**
```bash
ps aux                                  # listar processos
top                                     # monitorar tempo real
sleep 3600 &                            # background process
kill -15 PID                            # SIGTERM (graceful)
kill -9 PID                             # SIGKILL (force)
```

**10:00-10:45 (Logs):**
```bash
cat /var/log/auth.log                  # login attempts
grep "Failed" /var/log/auth.log        # failed logins
tail -f /var/log/syslog                # follow logs
```

**10:45-11:15 (Consolidação):**
- Documento: `signals_cheatsheet.md`

### QUINTA (27 Jan) - TCP/IP Model (Teórico)

**08:00-09:00 (Teoria):**
- 7 camadas OSI
- Modelo TCP/IP simplificado: Link → Internet → Transport → Application
- Cada camada tem seu próprio protocolo

**09:00-10:00 (Visual):**
- Desenhar modelo em papel ou Excalidraw
- Associar protocolo a cada camada
- Ex: Camada 2 = MAC, Camada 3 = IP, Camada 4 = TCP/UDP

**10:00-10:30 (Revisão):**
- Ler "Computer Networking: A Top-Down Approach" cap. 1

**10:30-11:00 (Quiz):**
- Qual camada é DNS? (Resposta: 7 - Application)
- SSH? (Resposta: 7 - Application)
- ARP? (Resposta: 2/3 - Data Link/Network)

### SEXTA (28 Jan) - Como a Internet Funciona (Básico)

**08:00-09:00 (Teoria):**
- DNS lookup
- IP routing
- Pacotes
- ISP

**09:00-10:00 (Prática):**
```bash
nslookup google.com              # resolve DNS
traceroute google.com            # ver caminho
ping google.com                  # testar conectividade
```

**10:00-10:45 (Python):**
```python
import socket
ip = socket.gethostbyname("google.com")
print(f"Google IP: {ip}")
```

**10:45-11:15 (Consolidação):**
- Notas: `week1_summary.md`

**11:15-11:50 (GitHub):**
- Commit: `Week 1 complete - Linux + TCP/IP intro`

---

## Semana 2 (31 Jan - 6 Fev): Linux Avançado + Python Fundamentos

### SEGUNDA (31 Jan) - Linux: Bash Scripts Básicos

**Teoria (60 min):** Variáveis, loops, condições em bash

**Prática (60 min):**
```bash
#!/bin/bash
# myip.sh
echo "Meu IP:"
hostname -I
```

```bash
chmod +x myip.sh
./myip.sh
```

**Consolidação (30 min):** Criar 3 scripts diferentes

**GitHub (35 min):** Commit scripts

### TERÇA (1 Fev) - Python: Variáveis e Tipos

**Teoria (60 min):** int, float, str, bool, type()

**Prática (60 min):**
```python
x = 5
print(type(x))              # <class 'int'>

msg = "Hello"
print(msg + " World")       # Hello World

num = int("42")
text = str(42)
```

**Revisão (30 min):** Quando usar cada tipo

### QUARTA (2 Fev) - Python: Estruturas de Controle

**Teoria (60 min):** if/elif/else, for, while

**Prática (60 min):**
```python
for i in range(10):
    print(i)

if x > 5:
    print("Maior")

count = 0
while count < 5:
    count += 1
```

**Secundário (45 min):** Linux: `find`, `grep`

**Consolidação (30 min):** Notas: `estruturas.md`

### QUINTA (3 Fev) - Python: Listas, Dicts, Tuples

**Teoria (60 min):** Coleções de dados

**Prática (60 min):**
```python
lista = [1, 2, 3]
print(lista[0])              # 1

dict = {"nome": "João"}
print(dict["nome"])          # João

tupla = (1, 2, 3)
for item in lista:
    print(item)
```

**Revisão (30 min):** Quando usar cada uma

### SEXTA (4 Fev) - Python: Funções

**Teoria (60 min):** def, parametros, return, *args, **kwargs

**Prática (60 min):**
```python
def greet(name):
    return f"Olá, {name}"

def add(a, b):
    return a + b

print(greet("João"))
print(add(2, 3))
```

**Consolidação (30 min):** Criar 5 funções úteis

**GitHub (35 min):** Commit: `Week 2 - Python basics`

---

## Semana 3 (7-13 Fev): Redes Fundamentais + Wireshark Intro

### SEGUNDA (7 Fev) - TCP (3-Way Handshake)

**Teoria (60 min):** SYN, SYN-ACK, ACK, números de sequência

**Prática (60 min):**
- Abrir Wireshark
- Capturar tráfego local
- Filtro: `tcp.flags.syn == 1`
- Ver handshake completo

**Secundário (45 min):** UDP basics

**Consolidação (30 min):** Desenhar handshake SYN → SYN-ACK → ACK

### TERÇA (8 Fev) - DNS e DHCP

**Teoria (60 min):** DNS query/response, DHCP allocation

**Prática (60 min):**
```bash
nslookup google.com         # enquanto Wireshark captura
```
- Ver pacotes DNS em Wireshark
- Filtro: `dns`

**Revisão (30 min):** Diferenças TCP vs UDP

### QUARTA (9 Fev) - SSH e Criptografia Básica

**Teoria (60 min):** SSH protocol, chaves pública/privada

**Prática (60 min):**
```bash
ssh-keygen -t rsa -b 4096
ssh user@host
ssh-keyscan -t rsa host
```

**Secundário (45 min):** HTTP vs HTTPS

**Consolidação (30 min):** Notas: `SSH_security.md`

### QUINTA (10 Fev) - ARP e Comunicação Local

**Teoria (60 min):** ARP protocol, MAC discovery

**Prática (60 min):**
```bash
arp -a                      # ver tabela ARP
ping 192.168.1.1           # gerar ARP
```

- Wireshark: filtro `arp`
- Ver ARP request/reply

**Revisão (30 min):** Risco: ARP spoofing

### SEXTA (11 Fev) - Wireshark Análise Profunda

**Teoria (60 min):** Filters, follow TCP stream, estatísticas

**Prática (60 min):**
- Filtros: `tcp port 22`, `ip.src == 192.168.1.1`
- Follow stream: direita → Follow TCP Stream
- Statistics → Protocol Hierarchy

**Consolidação (30 min):** Screenshot análise completa

**GitHub (35 min):** Commit: `Week 3 - Networks + Wireshark`

---

## Semana 4 (14-20 Fev): Endereçamento + Criptografia

### SEGUNDA (14 Fev) - IPv4 e Subnetting

**Teoria (60 min):** IPv4 format, máscara de rede, CIDR notation

**Prática (60 min):**
```bash
ifconfig                    # macOS/Linux
ipconfig /all              # Windows

# Cálculos
# 192.168.0.0/24 = 256 IPs (0-255)
# /16 = 65.536 IPs
# /8 = 16.777.216 IPs
```

**Secundário (45 min):** IPv6 basics

**Consolidação (30 min):** Tabela subnetting

### TERÇA (15 Fev) - Criptografia Simétrica

**Teoria (60 min):** Mesma chave encode/decode, AES, DES

**Prática (60 min):**
```bash
pip install pycryptodome
```

```python
from Crypto.Cipher import AES
# Script de encode/decode AES
```

**Revisão (30 min):** Por que DES é inseguro hoje

### QUARTA (16 Fev) - Criptografia Assimétrica (RSA)

**Teoria (60 min):** Pública/privada, RSA, por que é lento

**Prática (60 min):**
```python
from Crypto.PublicKey import RSA
key = RSA.generate(2048)
# Encrypt com pública, decrypt com privada
```

**Secundário (45 min):** SSH usa este conceito

**Consolidação (30 min):** Diagrama público/privado

### QUINTA (17 Fev) - Hashing

**Teoria (60 min):** One-way function, SHA-256, MD5, salt

**Prática (60 min):**
```python
import hashlib
hash = hashlib.sha256("password".encode()).hexdigest()
print(hash)
```

**Revisão (30 min):** Por que usar hashing para senhas

### SEXTA (18 Fev) - TLS/SSL e Certificados

**Teoria (60 min):** TLS handshake, certificados digitais, CA

**Prática (60 min):**
```bash
openssl s_client -connect google.com:443
```

- Wireshark: capturar HTTPS request
- Ver TLS handshake (Client Hello, Server Hello)

**Consolidação (30 min):** Notas: `TLS_complete.md`

**GitHub (35 min):** Commit: `Week 4 - Networks + Crypto`

---

## Semana 5 (21-27 Fev): OWASP Top 10 Intro + Python Avançado

### SEGUNDA (21 Fev) - SQL Injection + XSS (Teórico)

**Teoria (60 min):** Como SQL injection funciona, payloads

**Prática (60 min):**
```
Exemplo: ' OR '1'='1
Query fica: SELECT * WHERE user="" OR "1"="1"
Resultado: retorna TUDO
```

**Secundário (45 min):** XSS basics

**Consolidação (30 min):** Documentar payloads de exemplo

### TERÇA (22 Fev) - Broken Authentication

**Teoria (60 min):** Senhas fracas, session hijacking, credential stuffing

**Prática (60 min):**
- Como Burp intercepta cookies
- Modificar cookie em Burp e testar

**Revisão (30 min):** MFA como mitigação

### QUARTA (23 Fev) - Python: File I/O + JSON

**Teoria (60 min):** Ler/escrever arquivos, JSON parsing

**Prática (60 min):**
```python
with open("file.txt") as f:
    data = f.read()

import json
data = json.load(f)
json.dump(data, f)
```

**Secundário (45 min):** Wireshark export em JSON

**Consolidação (30 min):** Criar parser simples

### QUINTA (24 Fev) - Python: Requests (HTTP)

**Teoria (60 min):** HTTP requests library, métodos, headers

**Prática (60 min):**
```python
import requests
response = requests.get("https://httpbin.org/get")
print(response.status_code)
print(response.json())

requests.post("https://httpbin.org/post", data={"key": "value"})
```

**Revisão (30 min):** Diferença GET vs POST

### SEXTA (25 Fev) - Projeto: Análise de Tráfego Simples

**Teoria (60 min):** Scapy library - criar pacotes

**Prática (60 min):**
```bash
pip install scapy
```

```python
from scapy.all import *
# Criar e enviar pacote ICMP (ping customizado)
```

**Consolidação (30 min):** Documentação de projeto

**GitHub (35 min):** Commit: `Week 5 - OWASP intro + Python advanced`

---

## Semana 6 (28 Fev - 6 Mar): Consolidação FASE 1

### SEGUNDA (28 Fev) - Revisão Total: Linux

**Teoria (60 min):** Revisar: diretórios, permissões, processos, logs

**Prática (60 min):**
- Teste: criar usuário, dar permissões específicas, verificar logs

**Consolidação (30 min):** Quiz no papel: 20 questões Linux

### TERÇA (1 Mar) - Revisão Total: Python

**Teoria (60 min):** Tipos, controle, coleções, funções, I/O

**Prática (60 min):**
- Desafio: escrever script que lê JSON, processa, exporta

**Revisão (30 min):** Quiz: 15 questões Python

### QUARTA (2 Mar) - Revisão Total: Redes

**Teoria (60 min):** OSI, TCP/IP, protocolos, endereçamento

**Prática (60 min):**
- Wireshark: fazer DNS lookup, TCP connection, ping, tudo junto

**Consolidação (30 min):** Tabela: Protocolo | Camada | Porta | Uso

### QUINTA (3 Mar) - Revisão Total: Criptografia

**Teoria (60 min):** Simétrica, assimétrica, hashing, TLS

**Prática (60 min):**
- Teste: gerar chaves RSA, encriptar, descriptografar
- Hash: validar integridade de arquivo com SHA-256

**Revisão (30 min):** Quando usar cada tipo

### SEXTA (4 Mar) - Capstone FASE 1: Projeto Final

**Projeto:** Criar script Python que:
1. Captura pacotes com Scapy
2. Parseia alguns, extrai IPs, portas
3. Salva resultado em JSON
4. Exporta relatório em texto

**GitHub:** Commit: `Week 6 - FASE 1 Complete`

---

# FASE 2: INTERMEDIÁRIO (Semanas 7-14: 7 Mar - 1 Mai 2026)

## Objetivo
Explorar profundidade: Security+, Burp Suite, ferramentas profissionais, análise de tráfego real.

---

## Semana 7 (7-13 Mar): Security+ Intro + Burp Suite

### SEGUNDA (7 Mar) - Conceitos Security+ (CIA Triad)

**Teoria (60 min):** 
- **C**onfidentiality = dados não são lidos por pessoas erradas
- **I**ntegridade = dados não são modificados
- **A**disponibilidade = dados estão sempre acessíveis

**Prática (60 min):**
- Caso de estudo 1: Banco (CIA como é aplicado)
- Caso de estudo 2: Hospital (qual é mais importante?)

**Consolidação (30 min):** Documentar pensamento crítico

### TERÇA (8 Mar) - Vulnerabilidade vs Ameaça vs Risco

**Teoria (60 min):**
- **Vulnerabilidade** = fraqueza
- **Ameaça** = pessoa/coisa que pode explorar
- **Risco** = Vulnerabilidade + Ameaça
- Fórmula: Risk = Probability × Impact

**Prática (60 min):**
- Exemplo 1: Porta SSH aberta (vuln) + hacker (threat) = risco alto
- Exemplo 2: Typo em código (vuln) + ninguém sabe (threat baixa) = risco baixo

**Revisão (30 min):** Matrix de risco

### QUARTA (9 Mar) - Burp Suite Setup + Basics

**Teoria (60 min):** O que é Burp, arquitetura, módulos principais

**Prática (60 min):**
- Instalar Burp Community
- Configurar navegador proxy
- Capturar primeiro request em Intercept
- Modificar e enviar

**Secundário (45 min):** Repeater module

**Consolidação (30 min):** Notas: `Burp_quickstart.md`

### QUINTA (10 Mar) - Análise de Tráfego Anormal

**Teoria (60 min):** Baseline, anomalias, IDS/IPS conceitos

**Prática (60 min):**
- Wireshark: capturar tráfego normal (30 min)
- Wireshark: capturar tráfego port scan (30 min)
- Comparar: diferenças?

**Revisão (30 min):** Padrões a procurar

### SEXTA (11 Mar) - Projeto: Web Request Analyzer

**Projeto:** Python + Burp
- Exportar requisições do Burp
- Parser para extrair: URL, método, headers, parâmetros
- Identificar: GET vs POST, params, cookies
- Salvar relatório

**GitHub (35 min):** Commit: `Week 7 - Burp + Analysis`

---

## Semana 8 (14-20 Mar): OWASP Profundo + Nmap

### SEGUNDA (14 Mar) - SQL Injection Prático

**Teoria (60 min):** Tipos de SQL injection: blind, time-based, union-based

**Prática (60 min):**
- DVWA ou HackTheBox: executar SQL injection real
- Burp Intruder: testar payloads
- Entender prepared statements como proteção

**Secundário (45 min):** Blind SQL injection conceito

**Consolidação (30 min):** Documentar tipos de payloads

### TERÇA (15 Mar) - XSS Prático

**Teoria (60 min):** Stored, Reflected, DOM-based XSS

**Prática (60 min):**
- DVWA: testar XSS em formulário
- Burp: modificar requests para injetar JavaScript
- Ver como cookies são roubados

**Revisão (30 min):** Diferenças entre tipos

### QUARTA (16 Mar) - Nmap: Port Scanning

**Teoria (60 min):** Tipos de scans, flags, evasão

**Prática (60 min):**
```bash
nmap -sS target.com              # TCP SYN scan
nmap -sV target.com              # service version
nmap -A target.com               # aggressive
nmap -Pn target.com              # ignore ping
nmap -p 80,443 target.com        # portas específicas
```

**Secundário (45 min):** NSE scripts (Nmap Scripting Engine)

**Consolidação (30 min):** Tabela de scan types

### QUINTA (17 Mar) - Detecção de Scans

**Teoria (60 min):** IDS patterns, port scan signatures

**Prática (60 min):**
- Wireshark: capturar port scan
- Ver flags SYN sem ACK (fingerprint)
- Identificar pattern vs normal tráfego

**Revisão (30 min):** Threshold de detecção

### SEXTA (18 Mar) - Projeto: Network Mapper

**Projeto:** Python + Nmap
- Script que roda Nmap
- Parseia output
- Gera relatório com hosts, portas abertas
- Salva em JSON

**GitHub (35 min):** Commit: `Week 8 - OWASP + Nmap`

---

## Semana 9 (21-27 Mar): Metasploit + Password Cracking

### SEGUNDA (21 Mar) - Metasploit Framework Basics

**Teoria (60 min):** Arquitetura, payloads, encoders

**Prática (60 min):**
```bash
msfconsole
search ssh
use exploit/ssh/something
show options
set RHOSTS target.com
exploit
```

**Consolidação (30 min):** Notas: `msfconsole_basics.md`

### TERÇA (22 Mar) - Metasploit Prático

**Teoria (60 min):** Modules, post-exploitation

**Prática (60 min):**
- Executar exploit em máquina virtual
- Obter reverse shell
- Post-exploitation básica (whoami, ls, etc)

**Revisão (30 min):** Diferença entre payloads

### QUARTA (23 Mar) - Password Cracking: John

**Teoria (60 min):** Hash formats, wordlists, regras

**Prática (60 min):**
```bash
john --format=md5 hashes.txt
john --wordlist=rockyou.txt hashes.txt
john --show hashes.txt
```

**Secundário (45 min):** Rainbow tables conceito

**Consolidação (30 min):** Documentar técnicas

### QUINTA (24 Mar) - Password Cracking: Hashcat

**Teoria (60 min):** GPU acceleration, mask attacks

**Prática (60 min):**
```bash
hashcat -m 0 hashes.txt rockyou.txt     # MD5
hashcat -m 1000 hashes.txt rockyou.txt  # NTLM
hashcat -a 3 hashes.txt ?a?a?a?a       # bruteforce 4 chars
```

**Revisão (30 min):** GPU vs CPU speeds

### SEXTA (25 Mar) - Projeto: Hash Analyzer

**Projeto:** Python
- Identificar tipo de hash automaticamente
- Sugerir melhor ferramenta (John vs Hashcat)
- Integrar wordlist lookup
- Gerar relatório

**GitHub (35 min):** Commit: `Week 9 - Metasploit + Cracking`

---

## Semana 10 (28 Mar - 3 Abr): Scanners de Vulnerabilidade

### SEGUNDA (28 Mar) - OpenVAS/Nessus Basics

**Teoria (60 min):** Arquitetura, CVE database, scoring

**Prática (60 min):**
- Instalar OpenVAS (gratuito)
- Criar task
- Scanear máquina local
- Ver resultados

**Consolidação (30 min):** Entender CVSS scores

### TERÇA (29 Mar) - Interpretando Resultados

**Teoria (60 min):** Severity levels, false positives, remediation

**Prática (60 min):**
- Analisar relatório de scan
- Filtrar por severidade
- Pesquisar CVEs encontrados

**Revisão (30 min):** Diferença Critical vs High vs Medium

### QUARTA (30 Mar) - Wireshark Avançado: Estatísticas

**Teoria (60 min):** Protocol hierarchy, endpoints, conversations

**Prática (60 min):**
- Statistics → Protocol Hierarchy
- Statistics → Endpoints
- Statistics → IPv4 Statistics
- Identificar hosts e volume de tráfego

**Consolidação (30 min):** Screenshots análise

### QUINTA (31 Mar) - Detecção de Anomalias

**Teoria (60 min):** Baseline estabelecimento, outlier detection

**Prática (60 min):**
- Capturar 1h tráfego "normal"
- Capturar 1h com atividade suspeita (port scan, brute force)
- Comparar: diferenças?

**Revisão (30 min):** Threshold de alertas

### SEXTA (1 Abr) - Projeto: Vulnerability Report Generator

**Projeto:** Python + OpenVAS/Nessus
- Parse scan results
- Gera relatório profissional
- Prioriza por severity
- Recomendações de remediação

**GitHub (35 min):** Commit: `Week 10 - Scanners`

---

## Semana 11 (4-10 Abr): Security+ Aprofundado

### SEGUNDA (4 Abr) - Criptografia no Security+

**Teoria (60 min):** Protocolos, certificados, PKI

**Prática (60 min):**
- Gerar auto-signed certificate
- Converter formatos (PEM, DER, PKCS12)
- Ver detalhes com OpenSSL

**Consolidação (30 min):** Tabela protocolos criptográficos

### TERÇA (5 Abr) - Access Control Models

**Teoria (60 min):** DAC, MAC, RBAC, ABAC

**Prática (60 min):**
- Exemplos: Linux (DAC), militar (MAC), corporativo (RBAC)
- Implementar permissões em sistema

**Revisão (30 min):** Quando usar cada modelo

### QUARTA (6 Abr) - Threat Modeling

**Teoria (60 min):** STRIDE, PASTA, data flow diagrams

**Prática (60 min):**
- Desenhar DFD de aplicação simples
- Aplicar STRIDE: Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service, Elevation of Privilege

**Consolidação (30 min):** Documento threat model

### QUINTA (7 Abr) - Security+ Simulado

**Teoria (60 min):** Revisar tópicos principais

**Prática (60 min):**
- Fazer simulado prático (90 questões, 90 min)
- Revisar erros

**Revisão (30 min):** Focar em áreas fracas

### SEXTA (8 Abr) - Projeto: Threat Model Builder

**Projeto:** Python + Diagramas
- Entrada: descrever aplicação
- Saída: STRIDE matrix
- Relatório: riscos identificados

**GitHub (35 min):** Commit: `Week 11 - Security+`

---

## Semana 12 (11-17 Abr): Wireshark Avançado + Análise Profissional

### SEGUNDA (11 Abr) - Wireshark: Dissectors Customizados

**Teoria (60 min):** Lua scripts, protocolos custom

**Prática (60 min):**
- Criar dissector Lua simples
- Aplicar em capture
- Ver como Wireshark parseia

**Consolidação (30 min):** Documentação dissector

### TERÇA (12 Abr) - TCP/IP Deep Dive

**Teoria (60 min):** Sequence numbers, window size, MSS, TTL

**Prática (60 min):**
- Wireshark: analisar TCP flags em conexão
- Ver como window tamanho muda
- Entender flow control

**Revisão (30 min):** Attacks baseados em TCP: SYN flood

### QUARTA (13 Abr) - Detecção de Brute Force

**Teoria (60 min):** Padrões de SSH brute force, RDP, web

**Prática (60 min):**
- Wireshark: capturar brute force SSH
- Ver múltiplos SYN-RST (rejected connections)
- Identificar fonte e alvo

**Consolidação (30 min):** Signature de brute force

### QUINTA (14 Abr) - Detecção de DDoS

**Teoria (60 min):** Tipos: volumetric, protocol, application

**Prática (60 min):**
- Wireshark: capturar DDoS simulado
- Ver flood de pacotes
- Statistics → Endpoints (múltiplos IPs atacando)

**Revisão (30 min):** Threshold de DDoS

### SEXTA (15 Abr) - Projeto: Network Behavior Analysis Tool

**Projeto:** Python + Wireshark
- Captura contínua
- Baseline automático
- Alertas de anomalia
- Dashboard simples (CLI)

**GitHub (35 min):** Commit: `Week 12 - Wireshark Advanced`

---

## Semana 13 (18-24 Abr): Incident Response

### SEGUNDA (18 Abr) - Metodologia IR

**Teoria (60 min):** DETECT → RESPOND → MITIGATE → RECOVER

**Prática (60 min):**
- Estudar case study de incidente real
- Documentar timeline
- Identificar root cause

**Consolidação (30 min):** IR playbook template

### TERÇA (19 Abr) - Forensics Básico

**Teoria (60 min):** Chain of custody, preservação de evidência

**Prática (60 min):**
- dd (disk dump)
- Criar imagem forense
- Hash verificação (MD5, SHA256)

**Revisão (30 min):** Importância de chain of custody

### QUARTA (20 Abr) - Log Analysis

**Teoria (60 min):** Parsing, correlation, timeline

**Prática (60 min):**
```bash
grep "Failed" /var/log/auth.log | wc -l
grep "Failed" /var/log/auth.log | tail -100
awk '{print $1}' file.log | sort | uniq -c | sort -rn
```

**Consolidação (30 min):** Script de parsing

### QUINTA (21 Abr) - Relatório de Incidente

**Teoria (60 min):** Estrutura, linguagem profissional, recomendações

**Prática (60 min):**
- Escrever relatório de incidente fictício
- Incluir: timeline, impacto, remediação

**Revisão (30 min):** Feedback/review

### SEXTA (22 Abr) - Projeto: Incident Report Generator

**Projeto:** Python + Template
- Entrada: logs de incidente
- Saída: relatório profissional
- Inclui: timeline, root cause, recommendations

**GitHub (35 min):** Commit: `Week 13 - Incident Response`

---

## Semana 14 (25 Mai - 1 Mai): Consolidação FASE 2

### SEGUNDA (25 Abr) - Revisão Total: Ferramentas

**Teoria (60 min):** Wireshark, Burp, Nmap, Metasploit

**Prática (60 min):**
- Teste integrado: usar todas as ferramentas em conjunto

**Consolidação (30 min):** Cheatsheet de ferramentas

### TERÇA (26 Abr) - Revisão Total: Conceitos

**Teoria (60 min):** CIA, OWASP, Risk, Threat Modeling

**Prática (60 min):**
- Quiz: 50 questões Security+

**Revisão (30 min):** Focar em áreas fracas

### QUARTA (27 Abr) - Revisão Total: Análise

**Teoria (60 min):** Anomalia, brute force, DDoS, incidents

**Prática (60 min):**
- Wireshark: análise completa de tráfego misto

**Consolidação (30 min):** Assinatura de eventos

### QUINTA (28 Abr) - Capstone FASE 2: Projeto Integrado

**Projeto:** Tudo junto!
- Capturar tráfego com Wireshark
- Usar Nmap para descobrir hosts
- Burp para testar aplicação
- Gerar relatório profissional

**Revisão (30 min):** Auto-avaliação

### SEXTA (29 Abr) - Apresentação FASE 2

**GitHub (35 min):** Commit final FASE 2

---

# FASE 3: AVANÇADO (Semanas 15-20: 2 Mai - 13 Jun 2026)

## Objetivo
Análise profissional, detecção de anomalias complexas, cenários reais, ferramentas SIEM básicas.

> **Nota:** As semanas 15-20 seguem a mesma estrutura: 210 min seg/qua/sex + 160 min ter/qui.

---

## Semana 15: Análise Profissional de Tráfego

### SEGUNDA (2 Mai) - Captura 24/7

**Objetivo:** Estabelecer baseline contínuo

### TERÇA (3 Mai) - Anomaly Scoring

**Objetivo:** Criar sistema de pontuação para anomalias

### QUARTA (4 Mai) - Correlação de Eventos

**Objetivo:** Conectar múltiplos eventos (port scan → SSH brute → backdoor)

### QUINTA (5 Mai) - Baseline Refinement

**Objetivo:** Ajustar thresholds com dados reais

### SEXTA (6 Mai) - Projeto: 24/7 Monitor

**Objetivo:** Script que captura e analisa continuamente

---

## Semana 16: Detecção Avançada

### SEGUNDA (9 Mai) - Command & Control (C2) Detection

**Objetivo:** Identificar beacons e comunicação C2

### TERÇA (10 Mai) - Data Exfiltration Patterns

**Objetivo:** Detectar vazamento de dados

### QUARTA (11 Mai) - Lateral Movement

**Objetivo:** Identificar movimento lateral em rede

### QUINTA (12 Mai) - Persistence Mechanisms

**Objetivo:** Ver sinais de backdoors/persistência

### SEXTA (13 Mai) - Projeto: Threat Scorecard

**Objetivo:** Sistema de scoring de ameaças

---

## Semana 17: SIEM Básico (Splunk/ELK)

### SEGUNDA (16 Mai) - ELK Stack Installation

**Objetivo:** Setup Elasticsearch, Logstash, Kibana

### TERÇA (17 Mai) - Log Ingestion

**Objetivo:** Alimentar ELK com dados de Wireshark/syslog

### QUARTA (18 Mai) - Dashboards

**Objetivo:** Criar visualizações úteis

### QUINTA (19 Mai) - Alerting

**Objetivo:** Setup alertas automáticos

### SEXTA (20 Mai) - Projeto: Custom Dashboard

**Objetivo:** Dashboard profissional em ELK

---

## Semana 18: Malware Analysis Basics

### SEGUNDA (23 Mai) - Behavioral Analysis

**Objetivo:** Analisar tráfego de malware em sandbox

### TERÇA (24 Mai) - Network Indicators

**Objetivo:** Extrair IoCs (IPs, domains, hashes)

### QUARTA (25 Mai) - Timeline Reconstruction

**Objetivo:** Reconstruir ações de malware

### QUINTA (26 Mai) - Report Generation

**Objetivo:** Escrever relatório de análise

### SEXTA (27 Mai) - Projeto: Malware Traffic Parser

**Objetivo:** Extrair dados de PCAP de malware

---

## Semana 19: Threat Intelligence

### SEGUNDA (30 Mai) - IoC Correlation

**Objetivo:** Cruzar indicadores de múltiplas fontes

### TERÇA (31 Mai) - Threat Hunting

**Objetivo:** Procurar ativamente por ameaças conhecidas

### QUARTA (1 Jun) - ATT&CK Framework

**Objetivo:** Mapear ataques para MITRE ATT&CK

### QUINTA (2 Jun) - Campaign Tracking

**Objetivo:** Seguir campanhas de ataque

### SEXTA (3 Jun) - Projeto: Threat Intelligence Platform

**Objetivo:** Sistema de tracking de ameaças

---

## Semana 20: Consolidação FASE 3

### SEGUNDA (6 Jun) - Revisão Total

**Objetivo:** Review de tudo que aprendeu

### TERÇA (7 Jun) - Simulado Profissional

**Objetivo:** Análise completa como SOC analyst

### QUARTA (8 Jun) - Optimization

**Objetivo:** Melhorar detecções

### QUINTA (9 Jun) - Documentation

**Objetivo:** Documentar processos

### SEXTA (10 Jun) - Capstone FASE 3

**Objetivo:** Projeto grande integrando tudo

---

# FASE 4: CAPSTONE (Semanas 21-26: 13 Jun - 17 Jul 2026)

## Objetivo
Bug bounty, portfólio profissional, certificações finais, preparação para entrevistas.

---

## Semana 21: Bug Bounty Introduction

### SEGUNDA (13 Jun) - Plataformas (HackerOne, Bugcrowd)

**Objetivo:** Setup e primeiro programa

### TERÇA (14 Jun) - Methodology

**Objetivo:** Recon → Vulnerability Finding → Reporting

### QUARTA (15 Jun) - Report Writing

**Objetivo:** Escrever report profissional para programa

### QUINTA (16 Jun) - First Bug Hunt

**Objetivo:** Encontrar vulnerabilidade real

### SEXTA (17 Jun) - Projeto: Bug Bounty Tracker

**Objetivo:** Sistema de tracking de bugs encontrados

---

## Semana 22: Pentesting Methodology

### SEGUNDA (20 Jun) - Scoping & Reconnaissance

**Objetivo:** Fase 1 de pentesting

### TERÇA (21 Jun) - Scanning & Enumeration

**Objetivo:** Fase 2 de pentesting

### QUARTA (22 Jun) - Vulnerability Assessment

**Objetivo:** Fase 3 de pentesting

### QUINTA (23 Jun) - Exploitation

**Objetivo:** Fase 4 (com permissão!)

### SEXTA (24 Jun) - Projeto: Pentest Report

**Objetivo:** Relatório profissional completo

---

## Semana 23: Portfólio & Blog

### SEGUNDA (27 Jun) - GitHub Optimization

**Objetivo:** 10+ repos bem documentados

### TERÇA (28 Jun) - Blog Post Writing

**Objetivo:** 3-5 artigos técnicos

### QUARTA (29 Jun) - Video Tutorials

**Objetivo:** 2-3 vídeos de análise

### QUINTA (30 Jun) - LinkedIn Optimization

**Objetivo:** 1000+ followers, profile profissional

### SEXTA (1 Jul) - Projeto: Personal Website

**Objetivo:** Portfolio online

---

## Semana 24: Certificações Finais

### SEGUNDA (4 Jul) - Security+ Simulado Final

**Objetivo:** Fazer prova oficial ou simulado final

### TERÇA (5 Jul) - Wireshark Certified Analyst Prep

**Objetivo:** Preparar WCNA

### QUARTA (6 Jul) - GIAC Security Essentials

**Objetivo:** Estudar GSEC basics

### QUINTA (7 Jul) - Review de Todas

**Objetivo:** Decidir próximas certificações

### SEXTA (8 Jul) - Projeto: Certification Roadmap

**Objetivo:** Planejar próximas 12 meses

---

## Semana 25: Entrevistas Técnicas

### SEGUNDA (11 Jul) - Mock Interviews

**Objetivo:** Praticar respostas técnicas

### TERÇA (12 Jul) - Case Studies

**Objetivo:** Estudar e discutir casos reais

### QUARTA (13 Jul) - Behavioral Prep

**Objetivo:** Preparar soft skills

### QUINTA (14 Jul) - Salary Negotiation

**Objetivo:** Estudar ranges e estratégias

### SEXTA (15 Jul) - Projeto: Interview Prep Document

**Objetivo:** Guia pessoal de preparação

---

## Semana 26: FINAL CAPSTONE

### SEGUNDA (16 Jul) - Portfolio Review

**Objetivo:** Tudo pronto para mostrar

### TERÇA (17 Jul) - Celebração

**Objetivo:** Você completou! 🎉

---

# ✅ Checklist de Sucesso

- [ ] Estudar 3h30min todos os dias
- [ ] Fazer labs práticos (não só assistir vídeos)
- [ ] Documentar tudo no Obsidian
- [ ] Fazer commit GitHub 1x/semana MÍNIMO
- [ ] Revisar semana anterior antes de começar nova
- [ ] Fazer 1 projeto capstone por fase
- [ ] Escrever 3-5 artigos por fase (blog/Dev.to)
- [ ] Fazer simulados Security+ após semana 12
- [ ] Ter 10+ repositórios no GitHub ao final
- [ ] 1000+ seguidores no LinkedIn ao final
- [ ] 1 certificação obtida ao final (mínimo)

---

# 🎯 Dicas Finais

1. **Não pule PRÉ-ROADMAP** se tiver dúvidas em computação básica
2. **Faça labs DE VERDADE** - não é só ler/assistir
3. **Se travar em algo**, volte 1-2 tópicos, não pule
4. **Durma bem** e estude rested (3h30min > 6h cansado)
5. **Compartilhe aprendizado** (tweets, blog, vídeos)
6. **Encontre comunidade** (Discord, Reddit, grupos locais)
7. **Adapte à sua realidade** - se 210 min é muito, comece com 120 min
8. **Celebre pequenas vitórias** - cada semana é uma vitória!

---

## 📚 Recursos Recomendados

### Livros
- "Computer Networking: A Top-Down Approach" - Kurose & Ross
- "The Cyber Skills Roadmap" - CompTIA
- "Applied Network Security Monitoring" - Douglas

### Plataformas
- HackTheBox.com - labs práticos
- TryHackMe.com - cursos interativos
- SANS Cyber Aces - tutoriais grátis
- Malwarebytes Labs - análise malware

### Ferramentas (todas FREE)
- Wireshark - packet analysis
- Burp Suite Community - web testing
- Metasploit - exploitation
- Nmap - reconnaissance
- OpenVAS - vulnerability scanning
- ELK Stack - SIEM
- DVWA - vulnerable app for practice

---

**Boa sorte no roadmap! 🚀**

Comece segunda (17 de janeiro) e veja você mesmo evoluindo!
