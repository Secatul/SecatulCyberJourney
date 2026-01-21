
**Data de Início:** 17 de Janeiro de 2026  
**Data de Término:** 17 de Julho de 2026  
**Foco:** SOC Analyst → Pentester Junior (especialização Network Analysis)  
**Intensidade:** 7 dias/semana, ~3h30min/dia (210 min)  

---

## 📊 Distribuição de Tempo Diária (210 min = 3h30min)

```
ESTRUTURA BALANCEADA:

Seg/Qua/Sex (dias "completos" = 210 min):
  8:00-9:00   → Tópico Principal - TEORIA (60 min)
  9:00-10:00  → Tópico Principal - PRÁTICA/LAB (60 min)
  10:00-10:45 → Tópico Secundário - PRÁTICA (45 min)
  10:45-11:15 → Consolidação + Revisão (30 min)
  11:15-11:50 → Projetos + Publicação (35 min)
  ───────────────────────────
  Total: 210 min

Ter/Qui (dias "leves" = 160 min):
  8:00-9:00   → Tópico Principal - Continuação (60 min)
  9:00-10:00  → Prática/Lab do dia (60 min)
  10:00-10:30 → Livro + Wireshark (30 min)
  10:30-11:00 → Revisão (30 min)
  ───────────────────────────
  Total: 160 min

Sáb (dia "temático" = 150 min):
  9:00-10:30  → Tema Especial - Teoria (90 min)
  10:30-11:30 → Prática Profunda (60 min)

Dom (opcional - review = 60 min):
  Review da semana + documentação
```

**Total Semanal:** ~1400 min = 23h20min  
**Total 6 Meses:** ~560 horas reais de estudo

---

## 🎯 Estrutura em 4 Fases + PRÉ-ROADMAP

- **PRÉ-ROADMAP (Semana 0):** Computação Básica + Fundamentos Essenciais
- **FASE 1 (Semanas 1-6):** Fundações Sólidas - Linux, Python, Redes, Wireshark Básico
- **FASE 2 (Semanas 7-14):** Intermediário - Protocolos, Segurança, TryHackMe Sério, Security+ Profundo
- **FASE 3 (Semanas 15-20):** Avançado - Análise de Tráfego Profissional, Detecção de Anomalias, Projetos Complexos
- **FASE 4 (Semanas 21-26):** Capstone - Bug Bounty, Portfólio Final, Entrevistas

---

# PRÉ-ROADMAP: COMPUTAÇÃO BÁSICA + FUNDAMENTOS
## *"Antes de começar: entenda o que faz tudo funcionar"*

Se você já tem esses conhecimentos, **pule esta seção**. Senão, dedique **3-5 dias** antes de começar oficialmente a Semana 1.

---

## 0️⃣ COMPUTAÇÃO BÁSICA

### **Objetivo:** Entender funcionamento básico de computadores

#### **0.1 - Como o Computador Funciona?**
```
Checklist:
- [ ] Entender componentes físicos: CPU, GPU, RAM, HD/SSD
- [ ] Saber diferenciar software vs hardware
- [ ] Conhecer arquitetura Von Neumann
- [ ] Entender ciclo fetch-decode-execute
- [ ] Saber o que é clock/GHz em processadores
```

**Recursos:**
- YouTube: "How Computers Work" (Khan Academy)
- Tempo: 30 min

#### **0.2 - Sistema Binário**
```
Checklist:
- [ ] Entender representação binária (0s e 1s)
- [ ] Converter decimal → binário e vice-versa
- [ ] Entender bits e bytes
- [ ] Saber conceito de megabyte, gigabyte, terabyte
- [ ] Entender por que computadores usam binário
```

**Recursos:**
- Fundamentos Guia Anônima: "O que é Binário?"
- Tempo: 20 min

#### **0.3 - Software vs Hardware**
```
Checklist:
- [ ] Definir software (programas, sistemas operacionais)
- [ ] Definir hardware (componentes físicos)
- [ ] Entender interação software ↔ hardware
- [ ] Saber exemplos de cada um
- [ ] Compreender drivers e firmware
```

**Recursos:**
- YouTube: "Software vs Hardware" (Tech explainers)
- Tempo: 15 min

#### **0.4 - Como Funciona um Sistema Operacional?**
```
Checklist:
- [ ] Entender o papel do SO (intermediário entre user e hardware)
- [ ] Saber conceitos: processos, threads, memory management
- [ ] Entender scheduling de processos
- [ ] Compreender virtualização de memória
- [ ] Saber por que SO é essencial
```

**Recursos:**
- FreeCodeCamp: "Operating Systems Crash Course"
- Tempo: 45 min

#### **0.5 - x86 vs x64 vs ARM**
```
Checklist:
- [ ] Entender diferença entre arquiteturas
- [ ] Saber x86 = 32 bits, x64 = 64 bits
- [ ] Compreender ARM (processadores mobile)
- [ ] Saber implicações práticas (compatibilidade)
- [ ] Entender por que ARM está em ascensão
```

**Recursos:**
- YouTube: "x86 vs x64 vs ARM explained"
- Tempo: 20 min

---

## 1️⃣ REDES DE COMPUTADORES BASICS

### **Objetivo:** Fundação sólida em redes antes de TCP/IP detalhado

#### **1.1 - Como a Internet Funciona? (Overview)**
```
Checklist:
- [ ] Entender conceito de rede
- [ ] Saber o que é Internet vs Web
- [ ] Compreender ISP (Internet Service Provider)
- [ ] Entender backbone da internet
- [ ] Saber conceito básico de roteamento
```

**Recursos:**
- YouTube: "How Internet Works" (Kurzgesagt)
- Tempo: 20 min

#### **1.2 - IP vs MAC**
```
Checklist:
- [ ] Entender o que é IP (identificador lógico)
- [ ] Entender o que é MAC (identificador físico)
- [ ] Saber quando cada um é usado
- [ ] Compreender ARP (associação IP ↔ MAC)
- [ ] Entender por que precisamos dos dois
```

**Recursos:**
- YouTube: "IP vs MAC Address" (NetworkChuck)
- Tempo: 20 min

#### **1.3 - Rede Interna vs Externa**
```
Checklist:
- [ ] Entender conceito de LAN (Local Area Network)
- [ ] Entender conceito de WAN (Wide Area Network)
- [ ] Saber diferenças práticas
- [ ] Compreender gateway
- [ ] Entender DMZ (zona desmilitarizada)
```

**Recursos:**
- Fundamentos Guia Anônima: "Rede Interna vs Externa"
- Tempo: 20 min

#### **1.4 - Equipamentos de Rede Básicos**
```
Checklist:
- [ ] Entender o que faz um roteador
- [ ] Entender o que faz um switch
- [ ] Conhecer access point (WiFi)
- [ ] Saber conceito básico de firewall
- [ ] Entender modem
```

**Recursos:**
- YouTube: "Network Devices Explained"
- Tempo: 30 min

#### **1.5 - Protocolos Básicos Preview**
```
Checklist:
- [ ] Saber o que é protocolo (conjunto de regras)
- [ ] Entender HTTP (web) vs HTTPS (seguro)
- [ ] Saber o que é DNS (traduz nomes em IPs)
- [ ] Entender conceito de protocolo TCP vs UDP
- [ ] Saber portas básicas: 80 (HTTP), 443 (HTTPS), 53 (DNS), 22 (SSH)
```

**Recursos:**
- YouTube: "Network Protocols Explained"
- Tempo: 25 min

---

## 2️⃣ TERMINOLOGIA ESSENCIAL DE SEGURANÇA

### **Objetivo:** Vocabulário básico antes de estudar segurança profunda

#### **2.1 - O que é Segurança da Informação?**
```
Checklist:
- [ ] Definir SI (proteger informação contra acesso não autorizado)
- [ ] Entender diferença: SI vs Segurança Digital vs Segurança Cibernética
- [ ] Saber por que SI é importante
- [ ] Compreender escopo de SI
- [ ] Entender que SI é multidisciplinar
```

**Recursos:**
- Fundamentos Guia Anônima: "O que é SI?"
- Tempo: 20 min

#### **2.2 - CIA Triad (Confidencialidade, Integridade, Disponibilidade)**
```
Checklist:
- [ ] Confidencialidade = dados não são lidos por pessoas não autorizadas
- [ ] Integridade = dados não são alterados sem autorização
- [ ] Disponibilidade = dados/sistemas estão acessíveis quando necessário
- [ ] Entender como cada um se relaciona com criptografia
- [ ] Saber exemplos práticos de violações de cada um
```

**Recursos:**
- YouTube: "CIA Triad Explained" (Professor Messer)
- Tempo: 20 min

#### **2.3 - Vulnerabilidade vs Ameaça vs Risco**
```
Checklist:
- [ ] Vulnerabilidade = fraqueza em um sistema
- [ ] Ameaça = alguém/algo que pode explorar vulnerabilidade
- [ ] Risco = probabilidade × impacto
- [ ] Saber que nem toda vulnerabilidade é risco
- [ ] Entender relação: Vulnerabilidade + Ameaça = Risco
```

**Recursos:**
- Fundamentos Guia Anônima: "Vulnerabilidade vs Ameaça vs Risco"
- Tempo: 20 min

#### **2.4 - Exploit vs Payload**
```
Checklist:
- [ ] Exploit = código que explora vulnerabilidade
- [ ] Payload = dados/código que exploit entrega
- [ ] Entender exemplo prático (ex: SQL Injection + reverse shell)
- [ ] Saber que exploit sem payload é só teste
- [ ] Compreender diferença para pentesting ético
```

**Recursos:**
- YouTube: "Exploit vs Payload" (HackerSploit)
- Tempo: 15 min

#### **2.5 - Hacker vs Cracker vs Pentester**
```
Checklist:
- [ ] Hacker = alguém que encontra soluções criativas (neutro)
- [ ] Cracker = hacker com intenção maliciosa
- [ ] Pentester = profissional autorizado que testa segurança
- [ ] Entender diferença ética e legal
- [ ] Saber o espectro: White Hat → Gray Hat → Black Hat
```

**Recursos:**
- YouTube: "Hacker vs Cracker vs Pentester"
- Tempo: 15 min

#### **2.6 - OWASP Top 10 (Overview)**
```
Checklist:
- [ ] Injection (SQL, Command, etc)
- [ ] Broken Authentication
- [ ] Sensitive Data Exposure
- [ ] XML External Entities (XXE)
- [ ] Broken Access Control
- [ ] Security Misconfiguration
- [ ] Cross-Site Scripting (XSS)
- [ ] Insecure Deserialization
- [ ] Using Components with Known Vulnerabilities
- [ ] Insufficient Logging & Monitoring

Saber: O que é cada uma, exemplos básicos (detalhes vêm depois)
```

**Recursos:**
- YouTube: "OWASP Top 10 Overview" (Playlist)
- Tempo: 45 min

#### **2.7 - CVE vs CWE vs CVSS**
```
Checklist:
- [ ] CVE = vulnerabilidade específica identificada
- [ ] CWE = categoria de fraqueza
- [ ] CVSS = score de severidade (0-10)
- [ ] Saber onde encontrar CVEs (cve.mitre.org, nvd.nist.gov)
- [ ] Entender como usar essas informações
```

**Recursos:**
- Fundamentos Guia Anônima: "CVE e CWE"
- Tempo: 20 min

---

**Total PRÉ-ROADMAP:** ~5-6 horas (pode fazer em 2-3 dias)

---

# FASE 1: FUNDAÇÕES SÓLIDAS (Semanas 1-6)
## *"Aprender de verdade, não superficial"*

Objetivo: Entender PROFUNDAMENTE Linux, Python, TCP/IP Basics, Redes, Criptografia e primeiras análises com Wireshark.

---

## 📋 CHECKLIST COMPLETO - LINUX

### **Conhecimento Básico de Linux**
```
- [ ] Estrutura de diretórios: /, /home, /etc, /var, /tmp, /usr, /bin, /sbin
- [ ] Navegar: pwd, ls, ls -la, cd, cd -, cd ~
- [ ] Criar/Manipular arquivos: touch, mkdir, cp, mv, rm, rm -rf
- [ ] Entender propriedade de arquivos (user:group)
- [ ] Saber diferença entre shell e terminal
- [ ] Conhecer shells: bash, zsh, sh
```

**Semanas:** 1-2 (prática integrada)  
**Tempo:** ~10h

---

### **Gerenciamento de Permissões e Usuários**
```
- [ ] Conceito de usuário e grupo no Linux
- [ ] Ler permissões octal: 755, 644, 777
- [ ] chmod: mudar permissões (ex: chmod 755 arquivo)
- [ ] chown: mudar ownership (ex: chown user:group arquivo)
- [ ] sudo: elevação de privilégios
- [ ] Vulnerabilidades comuns (SUID, sudo misconfiguration)
- [ ] /etc/passwd e /etc/shadow (conceitual)
```

**Semanas:** 2-3 (prática integrada)  
**Tempo:** ~8h

---

### **Gerenciamento de Processos**
```
- [ ] Conceito de processo (PID, PPID)
- [ ] ps, ps aux, ps -ef
- [ ] top, htop (monitoramento)
- [ ] Foreground vs Background (&, jobs, fg, bg)
- [ ] Sinais: SIGTERM, SIGKILL, SIGHUP
- [ ] kill PID, kill -9 PID
- [ ] nice e renice (prioridade)
- [ ] Processos zumbis
```

**Semanas:** 2-3 (prática integrada)  
**Tempo:** ~6h

---

### **Logs e Monitoramento**
```
- [ ] /var/log/ estrutura básica
- [ ] syslog vs journald
- [ ] journalctl -u [service]
- [ ] tail, grep para análise de logs
- [ ] Logs importantes: auth, syslog, kern.log, secure
- [ ] Monitoramento de segurança (failed logins, etc)
```

**Semanas:** 4-5 (integrado em FASE 2)  
**Tempo:** ~6h

---

### **Gestão de Pacotes**
```
- [ ] APT (Debian/Ubuntu): apt-get, apt
- [ ] YUM/DNF (RedHat/CentOS)
- [ ] Instalação: apt install, apt update, apt upgrade
- [ ] Remover: apt remove, apt purge
- [ ] Buscar: apt search
- [ ] Conceito de repositórios
- [ ] Diferenças entre distros
```

**Semanas:** 3-4 (prática integrada)  
**Tempo:** ~5h

---

### **Scripts e Automação**
```
- [ ] Bash basics: variáveis, echo
- [ ] Estruturas de controle: if, for, while
- [ ] Functions em bash
- [ ] Pipes e redirecionamento: |, >, >>, <
- [ ] Cron jobs: crontab -e, syntax
- [ ] Automação de tarefas repetitivas
- [ ] Debugging scripts (set -x)
```

**Semanas:** 5-6 (integrado em FASE 1)  
**Tempo:** ~8h

---

### **Serviços e Systemd**
```
- [ ] systemctl start/stop/restart/status
- [ ] systemctl enable/disable
- [ ] journalctl para logs de serviços
- [ ] Arquivos .service básicos
- [ ] Configurar serviços SSH, Apache, etc
- [ ] Troubleshooting serviços
```

**Semanas:** 2-3 (prática integrada)  
**Tempo:** ~6h

---

**Total Linux FASE 1:** ~49 horas (distribuídas nas 6 semanas)

---

## 📋 CHECKLIST COMPLETO - REDES

### **Modelo OSI e TCP/IP**
```
Camada 1 (Física):
- [ ] Cabos, sinais elétricos
- [ ] Hub (dispositivo física)

Camada 2 (Data Link):
- [ ] MAC addresses (48 bits)
- [ ] Frames Ethernet
- [ ] Switches operam aqui
- [ ] ARP (Address Resolution Protocol)

Camada 3 (Network):
- [ ] IP (v4 e v6)
- [ ] Routers operam aqui
- [ ] Roteamento
- [ ] ICMP

Camada 4 (Transport):
- [ ] TCP (confiável, ordered)
- [ ] UDP (rápido, sem garantia)
- [ ] Portas

Camada 5-7 (Session, Presentation, Application):
- [ ] HTTP/HTTPS
- [ ] DNS
- [ ] FTP
- [ ] SSH
- [ ] SMTP, POP3, IMAP
```

**Semanas:** 1-2 (teoria + Wireshark)  
**Tempo:** ~12h

---

### **Protocolos Essenciais**
```
TCP (Camada 4):
- [ ] 3-way handshake: SYN, SYN-ACK, ACK
- [ ] Flags: SYN, ACK, FIN, RST, PSH
- [ ] Confiabilidade: checksums, sequencing
- [ ] Flow control: window size

UDP (Camada 4):
- [ ] Sem conexão, sem confiabilidade
- [ ] Mais rápido que TCP
- [ ] Uso: DNS, DHCP, gaming, streaming
- [ ] Quando não usar TCP

IPv4 vs IPv6:
- [ ] IPv4: 32 bits, notação decimal pontilhada (192.168.1.1)
- [ ] IPv6: 128 bits, notação hexadecimal (2001:db8::1)
- [ ] Diferenças práticas
- [ ] Migração IPv4 → IPv6

DNS (Port 53, UDP):
- [ ] Query → Server → Response
- [ ] Tipos de registro: A, AAAA, MX, CNAME, TXT, NS
- [ ] DNS spoofing, cache poisoning
- [ ] Wireshark: capturar e analisar DNS

ICMP (Ping):
- [ ] Diagnóstico de conectividade
- [ ] Echo Request/Reply
- [ ] Wireshark: ver estrutura ICMP

DHCP:
- [ ] Atribuição dinâmica de IP
- [ ] DISCOVER → OFFER → REQUEST → ACK
- [ ] Vulnerabilidades (DHCP starvation, rogue server)

ARP:
- [ ] Mapear IP → MAC na rede local
- [ ] ARP request/reply
- [ ] ARP spoofing, envenenamento ARP

SSH (Port 22, TCP):
- [ ] Acesso remoto seguro
- [ ] Autenticação: password, key-based
- [ ] Tunneling SSH

HTTP/HTTPS (Port 80/443):
- [ ] HTTP: GET, POST, PUT, DELETE, HEAD
- [ ] Status codes: 200, 301, 404, 500, etc
- [ ] Headers: Host, User-Agent, Authorization, Cookie
- [ ] HTTPS: criptografia TLS/SSL

TLS/SSL:
- [ ] Handshake TLS
- [ ] Certificados digitais
- [ ] Public key infrastructure (PKI)

FTP (Port 21):
- [ ] Active vs Passive mode
- [ ] Vulnerabilidades (credenciais em texto claro)

SMB/CIFS (Port 445):
- [ ] Compartilhamento de arquivos Windows
- [ ] Vulnerabilidades: EternalBlue, etc

Kerberos:
- [ ] Autenticação em redes Windows
- [ ] Tickets
- [ ] Pass-the-ticket attacks

SMTP/POP3/IMAP:
- [ ] Protocolos de email
- [ ] Diferenças práticas
```

**Semanas:** 2-8 (teoria + Wireshark capturando cada um)  
**Tempo:** ~20h

---

### **Endereçamento e Sub-redes**
```
IPv4:
- [ ] Notação decimal pontilhada: 192.168.1.1
- [ ] Classes: A, B, C, D, E
- [ ] Máscaras de sub-rede: /24, /25, /30
- [ ] CIDR notation: 192.168.0.0/24
- [ ] Calcular sub-redes manualmente
- [ ] Host bits vs Network bits
- [ ] IPv4 privado: 10.x.x.x, 172.16-31.x.x, 192.168.x.x

IPv6:
- [ ] Notação hexadecimal
- [ ] :: para zeros consecutivos
- [ ] Máscaras: /64, /48
- [ ] IPv6 link-local, site-local, global unicast
```

**Semanas:** 2-3 (prática com calculadoras + manualmente)  
**Tempo:** ~8h

---

### **Equipamentos de Rede**
```
Switch:
- [ ] Operação Layer 2
- [ ] MAC address table
- [ ] VLAN basics
- [ ] Port security

Router:
- [ ] Operação Layer 3
- [ ] Routing tables
- [ ] Static vs Dynamic routing
- [ ] Gateway padrão

Firewall:
- [ ] Stateful vs Stateless
- [ ] Rules: Allow/Deny
- [ ] Inbound vs Outbound
- [ ] NAT/PAT

Access Point (WiFi):
- [ ] SSID broadcasting
- [ ] Autenticação WiFi: WEP, WPA, WPA2, WPA3
- [ ] Canais e interferência

Modem:
- [ ] Conexão ISP
- [ ] Bridge mode vs Router mode

Load Balancer:
- [ ] Distribuição de tráfego
- [ ] Health checks
```

**Semanas:** 3-4 (teoria + conceitual)  
**Tempo:** ~6h

---

### **Análise de Tráfego com Wireshark**
```
Basics:
- [ ] Capturar pacotes
- [ ] Filtros básicos: tcp, udp, icmp, dns, arp
- [ ] Filtros avançados: tcp.port == 80, ip.src == x.x.x.x
- [ ] Seguir stream TCP: File → Follow TCP Stream
- [ ] Exportar objetos HTTP
- [ ] Salvar capturas (.pcap)

Análise de Protocolos:
- [ ] TCP 3-way handshake: ver SYN, SYN-ACK, ACK
- [ ] DNS query/response estrutura
- [ ] HTTP GET/POST em texto claro
- [ ] HTTPS: certificado, dados encriptados
- [ ] ARP request/reply

Estatísticas:
- [ ] Statistics → Endpoints
- [ ] Statistics → Conversations
- [ ] Statistics → Protocol Hierarchy
- [ ] Identificar hosts únicos, portas, protocolos

Detecção de Anomalias (depois em FASE 2):
- [ ] Port scans: muitos SYN, poucas respostas
- [ ] Brute force SSH: muitos RST flags
- [ ] DDoS patterns: muitos pacotes de mesma origem
- [ ] Data exfiltration: tráfego incomum
```

**Semanas:** 1-6 (integrado + Saturday Deep Dives)  
**Tempo:** ~18h

---

**Total Redes FASE 1:** ~64 horas (distribuídas nas 6 semanas)

---

## 📋 CHECKLIST COMPLETO - PROGRAMAÇÃO (Python)

### **Fundamentos**
```
- [ ] Variáveis e tipos de dados: int, float, str, bool
- [ ] Operadores: aritméticos, comparação, lógicos
- [ ] Print, input, type()
- [ ] Estruturas de controle: if, elif, else
- [ ] Loops: for, while
- [ ] Break, continue, pass
- [ ] Compreensão de listas: [x for x in range(10)]
```

**Semanas:** 1-2 (teoria + Exercism)  
**Tempo:** ~8h

---

### **Estruturas de Dados**
```
Lists:
- [ ] Criação, indexação, slicing
- [ ] append, extend, insert, remove, pop
- [ ] Iteração com for
- [ ] List comprehension

Tuples:
- [ ] Imutabilidade
- [ ] Unpacking: x, y = tupla
- [ ] Quando usar vs lists

Dictionaries:
- [ ] Key-value pairs
- [ ] Acesso: dict[key]
- [ ] Iteração: .items(), .keys(), .values()
- [ ] .get(), .pop(), .update()

Sets:
- [ ] Elementos únicos
- [ ] Operações: union, intersection, difference
```

**Semanas:** 2-3 (prática com Exercism)  
**Tempo:** ~8h

---

### **Funções e Módulos**
```
Funções:
- [ ] Definir: def nome(parametros):
- [ ] Return values
- [ ] Default parameters
- [ ] *args e **kwargs
- [ ] Docstrings
- [ ] Escopo: local vs global

Módulos e Imports:
- [ ] import modulo
- [ ] from modulo import funcao
- [ ] Módulos built-in: os, sys, json, datetime, math
- [ ] Estrutura de projeto
```

**Semanas:** 2-3 (prática com scripts)  
**Tempo:** ~8h

---

### **File I/O e Tratamento de Erros**
```
File Operations:
- [ ] open(filename, mode): 'r', 'w', 'a', 'rb', 'wb'
- [ ] read(), readlines(), write(), writelines()
- [ ] with statement (context manager)
- [ ] File seeking, tell()

JSON:
- [ ] json.load(), json.dump()
- [ ] json.loads(), json.dumps()
- [ ] Serialização e desserialização

CSV:
- [ ] csv.reader(), csv.writer()
- [ ] Parsing CSV files

Error Handling:
- [ ] try/except/finally
- [ ] raise exceções
- [ ] Custom exceptions
- [ ] Debugging com print statements
```

**Semanas:** 3-4 (prática com arquivos reais)  
**Tempo:** ~8h

---

### **Automação e Scripts**
```
- [ ] Scripts simples de automação
- [ ] Parsing de arquivos de configuração
- [ ] Processamento em lote
- [ ] Interação com arquivos/diretórios
- [ ] Subprocessos: subprocess.run(), os.system()
- [ ] Tratamento de argumentos: sys.argv, argparse
```

**Semanas:** 4-5 (integrado em projetos)  
**Tempo:** ~8h

---

### **Bibliotecas de Rede (intro)**
```
Requests:
- [ ] requests.get(), .post(), .put(), .delete()
- [ ] Headers, parameters, JSON body
- [ ] Response.status_code, .text, .json()
- [ ] Error handling

Socket (básico):
- [ ] socket.socket()
- [ ] Conectar a servidor
- [ ] Enviar/receber dados
- [ ] Conceitos de protocolo

Scapy (intro):
- [ ] Criar pacotes IP, TCP, UDP
- [ ] Enviar pacotes customizados
- [ ] Capturar pacotes (sniffing)
- [ ] Análise de respostas
```

**Semanas:** 5-6 (integrado em FASE 2)  
**Tempo:** ~10h

---

### **Projetos Práticos FASE 1**
```
Semana 1-2:
- [ ] Script que lê arquivo e conta palavras

Semana 2-3:
- [ ] Script que faz requisições HTTP e salva em JSON

Semana 3-4:
- [ ] Script que faz parse de logs

Semana 4-5:
- [ ] Script que automatiza uma tarefa repetitiva

Semana 5-6:
- [ ] Script que usa Scapy para enviar pacotes customizados
```

**Tempo:** ~10h (distribuído)

---

**Total Python FASE 1:** ~60 horas (distribuídas nas 6 semanas)

---

## 📋 CHECKLIST COMPLETO - CRIPTOGRAFIA

### **Fundamentos**
```
- [ ] Por que criptografia importa em SI
- [ ] Conceito: plaintext → ciphertext → plaintext
- [ ] Chave criptográfica
- [ ] Algoritmo vs implementação
```

**Semanas:** 4 (integrado em Security+ Ch 3)  
**Tempo:** ~4h

---

### **Criptografia Simétrica**
```
- [ ] Mesma chave para criptografar e descriptografar
- [ ] Rápida, eficiente
- [ ] Desafio: compartilhamento de chave
- [ ] Algoritmos: AES, DES, 3DES, RC4

AES (Advanced Encryption Standard):
- [ ] Tamanho de chave: 128, 192, 256 bits
- [ ] Modo: ECB, CBC, CFB, OFB, CTR
- [ ] Padrão NIST desde 2001
- [ ] Seguro (ainda em 2026)

DES/3DES:
- [ ] Algoritmo antigo (DES deprecated)
- [ ] 3DES: aplicar DES 3x (melhor segurança)
- [ ] Por que não usar mais DES puro
```

**Semanas:** 4 (theory + concepts)  
**Tempo:** ~6h

---

### **Criptografia Assimétrica (Public Key)**
```
Conceitos:
- [ ] Duas chaves: pública (compartilhada) + privada (secreta)
- [ ] Lenta comparada a simétrica
- [ ] Uso: troca de chaves, assinatura digital

RSA:
- [ ] Baseado em fatoração de números primos
- [ ] Tamanho de chave: 1024, 2048, 4096 bits
- [ ] Aplicações: SSH, SSL/TLS, PGP

Elliptic Curve Cryptography (ECC):
- [ ] Baseado em curvas elípticas
- [ ] Chaves menores que RSA com segurança equivalente
- [ ] Uso crescente: TLS 1.3, Signal, etc

Troca de Chaves Diffie-Hellman:
- [ ] Protocolo para concordar chave compartilhada
- [ ] Man-in-the-Middle vulnerability
```

**Semanas:** 4-5  
**Tempo:** ~8h

---

### **Hashing**
```
Conceitos:
- [ ] One-way function (não é reversível)
- [ ] Hash sempre mesmo tamanho
- [ ] Pequena mudança = hash completamente diferente
- [ ] Determinístico

Algoritmos:
- [ ] MD5: 128 bits (DEPRECATED - vulnerável)
- [ ] SHA-1: 160 bits (DEPRECATED para criptografia)
- [ ] SHA-256: 256 bits (SEGURO)
- [ ] SHA-512: 512 bits (mais seguro)

Aplicações:
- [ ] Verificação de integridade (checksums)
- [ ] Armazenamento de passwords
- [ ] Assinatura digital
- [ ] Prova-de-trabalho (blockchain)

Salt e Pepper:
- [ ] Salt: aleatório adicionado antes de hash
- [ ] Pepper: constante secreta adicionada
- [ ] Protege contra rainbow tables
- [ ] PBKDF2, bcrypt, scrypt usam salt
```

**Semanas:** 4-5  
**Tempo:** ~8h

---

### **Certificados e PKI**
```
Conceitos:
- [ ] Certificado = chave pública + metadados + assinatura
- [ ] X.509 formato padrão
- [ ] PKI = infraestrutura de gerenciar certificados

Componentes PKI:
- [ ] CA (Certificate Authority): emite certificados
- [ ] RA (Registration Authority): valida requisições
- [ ] Repository: armazena certificados

Validação de Certificado:
- [ ] Verificar assinatura CA
- [ ] Verificar data de expiração
- [ ] Verificar revogação (CRL, OCSP)
- [ ] Verificar Common Name (CN)

HTTPS/TLS:
- [ ] Cliente verifica certificado do servidor
- [ ] Chave pública do servidor
- [ ] Negociação de cipher suite
- [ ] Sessão encriptada com chave simétrica
```

**Semanas:** 5-6  
**Tempo:** ~8h

---

**Total Criptografia FASE 1:** ~34 horas (distribuídas nas semanas 4-6)

---

## 📅 SEMANA 1: Começar do Zero + Linux Basics

### **Segunda-feira (dia 1) - Linux Introduction I**

**Tema da Semana:** Linux Foundation + Estrutura do SO

**Seg 8:00-9:00 | TEORIA (60 min) - "O que é Linux"**
- Ler: Linux Basics (Udemy course notes OU LabEx intro)
- Tópicos:
  - Origem do Linux (Unix, GPL)
  - Distribuições (Debian, Ubuntu, CentOS)
  - Kernel vs Shell vs GNU
  - Arquitetura de diretórios (`/`, `/home`, `/etc`, `/var`, `/usr`)
- **Entender:** Não só "clicar", mas saber por que cada diretório existe
- Documento: Criar arquivo `semana1_notas_linux.txt`

**Seg 9:00-10:00 | LAB (60 min) - LabEx Linux Basics**
- LabEx: "Linux Basics" module
- Tarefas:
  1. Abrir terminal
  2. Navegar estrutura (`pwd`, `ls -la`, `cd`)
  3. Criar arquivos/pastas (`touch`, `mkdir`, `rm`)
  4. Entender permissões iniciais (`ls -l`)
- **Checkpoint:** Conseguir navegar sem cheat sheet

**Seg 10:00-10:45 | PRÁTICA (45 min) - Python Hello World**
- Tópico: Sintaxe básica Python
- Exercícios:
  - Instalar Python3 (SE não tem)
  - Primeiro script: `print("Hello, World!")`
  - Variáveis: `nome = "seu_nome"`, `idade = 20`
  - Tipos de dados: `type(nome)`, `type(idade)`
  - Primeiro loop: `for i in range(5): print(i)`
- **Output:** Script `hello.py` em ~/Documents/

**Seg 10:45-11:15 | CONSOLIDAÇÃO (30 min)**
- Revisar comandos Linux aprendidos
- Testar 3 comandos novos aleatoriamente
- Documentar: "5 coisas que aprendi hoje"

**Seg 11:15-11:50 | PROJETOS (35 min)**
- Criar GitHub repo: `meu-roadmap-2026`
- Adicionar: `semana1_notas_linux.txt` + `hello.py`
- Commit + Push
- Post LinkedIn: "Dia 1 do roadmap! ✅ Aprendendo Linux e Python"

---

### **Terça-feira (dia 2) - Python Basics I**

**Ter 8:00-9:00 | TEORIA (60 min) - Variáveis, Tipos, Lógica**
- FreeCodeCamp: Python for Beginners (0:00 - 1:00:00)
- Tópicos profundos:
  - String: concatenação, f-strings, slicing
  - Números: int, float, operações matemáticas
  - Booleano: True/False, comparações (`==`, `!=`, `>`, `<`)
  - Lógica: `and`, `or`, `not`
- **Entender:** Por que tipos importam em segurança?
- Documento: Criar `python_cheatsheet_semana1.md`

**Ter 9:00-10:00 | LAB (60 min) - Exercism (Python Track)**
- Exercism: 3 exercícios
  1. Hamming (strings + comparação)
  2. Grains (potências, lógica)
  3. Acronym (strings + loops)
- **Objetivo:** Entender sintaxe, NÃO apenas copiar
- Documentar soluções em arquivo

**Ter 10:00-10:30 | WIRESHARK (30 min) - Primeiros Passos**
- Livro "Análise de Tráfego TCP/IP" - Introdução (15 min)
  - Ler: "O que é um pacote?"
  - Conceito: Wireshark captura pacotes da rede
  - Por que analisar? (segurança, troubleshooting, aprendizado)
- Wireshark Prático (15 min):
  - Baixar Wireshark (se não tem)
  - Instalar
  - Abrir
  - Reconhecer interface (Packet List, Packet Details, Packet Bytes)
  - **Não capturar ainda**, só entender UI

**Ter 10:30-11:00 | REVISÃO (30 min)**
- Quiz mental: 5 conceitos de Python aprendidos
- Testar script Exercism novamente
- Verificar instalação Wireshark

---

### **Quarta-feira (dia 3) - Linux Basics II + TryHackMe Intro**

**Qua 8:00-9:00 | TEORIA (60 min) - Usuários, Permissões, Comandos Avançados**
- LabEx: User & Permission Management (teórico)
- Tópicos:
  - `whoami`, `id`, `groups`
  - Permissões: `rwx` (read, write, execute)
  - Ownership: user:group
  - `chmod`, `chown` basics
  - Processos: `ps`, `top`, `ps aux`
  - Kill vs Terminate
- Documento: Arquivo `linux_usuarios_permissoes.md`

**Qua 9:00-10:00 | LAB (60 min) - LabEx + Prática Manual**
- LabEx: "User & Permission" hands-on (30 min)
- Prática manual (30 min):
  - Criar novo usuário: `sudo useradd testuser`
  - Ver permissões: `ls -la /home/testuser/`
  - Mudar permissão: `chmod 755 arquivo.txt`
  - Testar acesso de arquivo com outro usuário
  - Matar processo: `kill PID`
- **Checkpoint:** Entender permissões octal (755, 644, etc)

**Qua 10:00-10:45 | PRÁTICA (45 min) - TryHackMe Room**
- TryHackMe: "Intro to Cyber Security" (começar)
  - Ler introdução
  - Completar seção 1: "What is Cybersecurity?"
  - Completar seção 2: "Careers in Cyber"
  - Responder 5 questões
- Documentar: Por que escolheu trilha SOC → Pentester?

**Qua 10:45-11:15 | CONSOLIDAÇÃO (30 min)**
- Revisar permissões Linux
- Testar 2 comandos novos de processos
- Revisão rápida Python

**Qua 11:15-11:50 | PROJETOS (35 min)**
- Adicionar ao GitHub: Notas das 3 aulas
- Commit: "Semana 1, dias 1-3: Linux basics + Python intro"
- Post LinkedIn: "3 dias in! Dominando Linux permissions 🔐"

---

### **Quinta-feira (dia 4) - Python + Redes Intro**

**Qui 8:00-9:00 | TEORIA (60 min) - Redes 101: OSI Model**
- FreeCodeCamp: Networking Course (Network Basics)
  OU Cybrary: CompTIA Security+ (Network Architecture)
- Tópicos:
  - OSI Model 7 camadas (teoria visual)
  - Camada 1 (Física): cabos, sinais
  - Camada 2 (Data Link): MAC, ARP
  - Camada 3 (Network): IP, routing
  - Camada 4 (Transport): TCP, UDP, portas
  - Camada 5-7: Sesión, Apresentação, Aplicação
  - Conceito: Cada camada tem seu trabalho
- Documento: `osi_model_explained.md`
- **Visual:** Desenhar diagrama OSI com responsabilidades

**Qui 9:00-10:00 | LAB (60 min) - Comandos de Rede Linux**
- Terminal Linux: Explorar rede
  - `ifconfig` ou `ip addr` - ver IP local
  - `ping google.com` - testar conectividade
  - `netstat -an` ou `ss -an` - ver portas abertas
  - `nslookup google.com` - DNS lookup
  - `route -n` - ver routing table
  - `arp -a` - ver cache ARP
- Documentar: Seu IP local, gateway, DNS
- **Entender:** Cada comando mostra parte diferente da rede

**Qui 10:00-10:30 | WIRESHARK (30 min) - Primeira Captura**
- Prática:
  1. Abrir Wireshark
  2. Selecionar interface (eth0, wlan0)
  3. Clicar "Start capture"
  4. Fazer `ping google.com` em outro terminal
  5. Parar captura (Stop button)
  6. Ver pacotes ICMP listados
  7. Clicar em 1 pacote, ver estrutura
- **Checkpoint:** Ver pacote ping completo (origem, destino, protocol)
- Documentar: Quantos pacotes em um ping? Qual é a estrutura?

**Qui 10:30-11:00 | REVISÃO (30 min)**
- Rever OSI Model
- Testar 3 comandos de rede
- Review Wireshark: Interface é clara?

---

### **Sexta-feira (dia 5) - Consolidação Semana 1**

**Sex 8:00-9:00 | TEORIA (60 min) - Security+ Chapter 1: Security Basics**
- CompTIA Security+: Ch 1 (Official Study Guide OU Cybrary)
- Tópicos:
  - Confidentiality, Integrity, Availability (CIA Triad)
  - Authentication vs Authorization
  - Risk Management basics
  - Threat vs Vulnerability
  - Common attack types (overview)
- Documento: `security_basics.md`

**Sex 9:00-10:00 | LAB (60 min) - Prática Integrada**
- Linux: Executar 10 comandos aprendidos sem cheat sheet
  - Navegar, criar arquivos, mudar permissões, ver rede
  - Documentar cada um
- Python: Reescrever Exercism #3 de memória
- Wireshark: Capturar ping novamente, documentar o que vê

**Sex 10:00-10:45 | PRÁTICA (45 min) - TryHackMe**
- TryHackMe: "Intro to Cyber Security" (terminar)
  - Completar seção 3: "Security Tools"
  - Completar seção 4: "Careers in Cyber" (final)
  - Responder restante das questões
- Screenshot da conclusão

**Sex 10:45-11:15 | CONSOLIDAÇÃO (30 min)**
- Revisão GERAL de Semana 1
  - 5 comandos Linux principais?
  - OSI Model? (desenhar de memória)
  - Conceitos Python? (variáveis, loops, tipos)
  - Wireshark: consegue capturar ping?
  - CIA Triad: consegue explicar?

**Sex 11:15-11:50 | PROJETOS (35 min)**
- Atualizar GitHub:
  - Pasta `semana1/` com todas as notas
  - README explicando o que aprendeu
  - Links dos recursos usados
- Commit: "Semana 1 COMPLETA - Linux, Python, Redes, Wireshark"
- Post LinkedIn (conteúdo + thread):
  ```
  "Semana 1 FINALIZADA ✅
  
  Aprendemos:
  - Linux: Diretórios, permissões, comandos
  - Python: Tipos, loops, Exercism 3/3
  - Redes: OSI Model, comandos de rede
  - Wireshark: Primeira captura de ICMP
  - Security: CIA Triad + basics
  
  Próxima semana: TCP/UDP, DNS, HTTP 🔍"
  ```

---

### **Sábado (dia 6) - Deep Dive: TCP/IP Foundations**

**Sab 9:00-10:30 | TEORIA (90 min) - TCP/IP Protocol Suite**
- Livro "Análise de Tráfego TCP/IP" - Capítulo 1-2 (completo)
- Recursos extras: CompTIA Security+ Ch2 (OSI/TCP-IP)
- Tópicos profundos:
  - Diferença OSI vs TCP/IP model
  - TCP/IP stack: Application, Transport, Internet, Link
  - Pacote IP: header, versão, TTL, flags
  - TCP vs UDP: handshake, confiabilidade, speed
  - Ports bem-conhecidos: 22 (SSH), 80 (HTTP), 443 (HTTPS), 53 (DNS), 3306 (MySQL)
- Documento: `tcp_ip_protocol_suite.md` (detalhado)
- **Visual:** Diagrama de pacote TCP/IP

**Sab 10:30-11:30 | PRÁTICA (60 min) - Wireshark Profundo**
- Wireshark Lab (extended):
  1. Capturar ping google.com (ICMP)
     - Expandir: Ethernet, IP, ICMP
     - Ver valores: TTL=64, Protocol=1
  2. Capturar `curl http://example.com` (HTTP)
     - Expandir: TCP 3-way handshake (SYN, SYN-ACK, ACK)
     - Ver GET request
     - Ver HTTP response
  3. Capturar `nslookup google.com` (DNS)
     - Filtro: `dns`
     - Ver DNS query (tipo A)
     - Ver DNS response (IP)
  4. ARP: `ping` na mesma rede
     - Ver ARP Request/Reply
- Documentar TUDO em arquivo `wireshark_dia6_lab.md`
- **Checkpoint:** Consegue explicar o que vê em cada pacote?

---

### **Domingo (dia 7) - Review + Documentação**

**Dom 11:00-12:00 | REVIEW (60 min)**
- Rever toda Semana 1
- Quiz:
  1. Explicar OSI Model (7 camadas)
  2. Desenhar TCP/IP packet
  3. Listar 10 comandos Linux + o que fazem
  4. Python: tipos de dados, diferença entre `==` e `=`
  5. Wireshark: como fazer captura, como filtrar
- Documentar respostas

---

### **✅ Marcos de Sucesso - Semana 1**

```
Linux:
- [ ] 15+ comandos sem cheat sheet
- [ ] Entender permissões octal (755, 644)
- [ ] Conseguir mudar arquivo de ownership
- [ ] Saber diferença entre / /home /etc /var

Python:
- [ ] 3+ exercícios Exercism completos
- [ ] Escrever script com strings, loop, variáveis
- [ ] Entender print(), input(), type()

Redes:
- [ ] OSI Model: 7 camadas + responsabilidades
- [ ] TCP vs UDP: diferenças principais
- [ ] 5+ comandos de rede (ping, ifconfig, netstat, nslookup, arp)
- [ ] Portas: 22, 80, 443, 53, 3306

Wireshark:
- [ ] Conseguir capturar pacotes ICMP
- [ ] Visualizar pacote completo (expandir camadas)
- [ ] Ver 3-way handshake TCP
- [ ] Ver DNS query/response
- [ ] Entender ARP

Security:
- [ ] CIA Triad: explicar Confidentiality, Integrity, Availability
- [ ] Auth vs Authz: diferença
- [ ] TryHackMe "Intro" completo

Projetos/Publicação:
- [ ] GitHub repo criado + 1 commit
- [ ] 1 post LinkedIn publicado
- [ ] Documentação em `semana1/` pronta
```

---

## 📅 SEMANA 2: Linux Avançado + Python Estruturas

# FASE 2: INTERMEDIÁRIO - Protocolos + Segurança (Semanas 7-14)

*8 semanas para:*
- Completar Security+ Chapters 4-8 (profundidade)
- Livro "Análise" Capítulos 4-7 (protocolos avançados, anomalias)
- TryHackMe: 5-8 rooms (Network, Linux, Web)
- Python: Scapy, requests, scripts de segurança
- Wireshark: Detectar anomalias, port scans, brute force

**Mesma estrutura das semanas 1-6, expandindo para:**

---

## 📋 CHECKLIST FASE 2 - SEGURANÇA OFENSIVA

### **OWASP Top 10 Profundamente**
```
1. Injection (SQL, Command, LDAP, etc):
   - [ ] SQL Injection: WHERE 1=1, UNION based
   - [ ] Detecção em Wireshark
   - [ ] SQLMap basics
   - [ ] Impacto: confidencialidade, integridade

2. Broken Authentication:
   - [ ] Weak credentials
   - [ ] Session fixation
   - [ ] Credential stuffing
   - [ ] Detecção: Burp Suite, manual testing

3. Sensitive Data Exposure:
   - [ ] Dados em texto claro (HTTP vs HTTPS)
   - [ ] Criptografia fraca
   - [ ] Exposição de backups
   - [ ] Impacto: confidencialidade

4. XML External Entities (XXE):
   - [ ] Exploração de XML parsers
   - [ ] File disclosure
   - [ ] SSRF via XXE
   - [ ] Remediação

5. Broken Access Control (iDOR):
   - [ ] Acesso a recursos não autorizados
   - [ ] Horizontal: acessar recurso de outro usuário
   - [ ] Vertical: acesso sem permissão apropriada
   - [ ] Detecção manual, Burp Repeater

6. Security Misconfiguration:
   - [ ] Default credentials
   - [ ] Diretórios expostos (.git, .env, backup files)
   - [ ] Headers de segurança ausentes
   - [ ] Versão de software exposta

7. Cross-Site Scripting (XSS):
   - [ ] Stored XSS (persistente)
   - [ ] Reflected XSS (não-persistente)
   - [ ] DOM XSS
   - [ ] Impacto: sessão, roubo de cookies

8. Insecure Deserialization:
   - [ ] Deserializar objetos não confiáveis
   - [ ] RCE potencial
   - [ ] Java, Python, PHP vulnerable

9. Using Components with Known Vulnerabilities:
   - [ ] Manter dependências atualizadas
   - [ ] Scanning com OWASP Dependency-Check
   - [ ] CVE tracking

10. Insufficient Logging & Monitoring:
    - [ ] Sem logs de eventos críticos
    - [ ] Sem alertas de anomalias
    - [ ] Logs não são persistentes
```

**Semanas:** 8-12 (teórico + prático)  
**Tempo:** ~20h

---

### **Detecção de Anomalias em Wireshark**
```
Port Scans:
- [ ] Muitos SYN para diferentes portas
- [ ] Poucas/nenhuma resposta SYN-ACK
- [ ] TTL decreasing
- [ ] Filtro: tcp.flags.syn == 1 AND tcp.flags.ack == 0

Brute Force SSH/RDP:
- [ ] Muitas tentativas de conexão
- [ ] Muitos RST (reset) flags = autenticação rejeitada
- [ ] Source IP único, destination única
- [ ] Filtro: tcp.port == 22 AND tcp.flags.rst == 1

DDoS:
- [ ] Muitos pacotes de mesma origem
- [ ] Tráfego anormalmente alto
- [ ] Mesmo payload repetido
- [ ] Statistics → Endpoints (ver topo)

Data Exfiltration:
- [ ] Tráfego saindo para IPs desconhecidos
- [ ] Conexões para portas incomuns
- [ ] Muitos dados saindo, poucos entrando

Malware Communication:
- [ ] Conexões para IPs maliciosos
- [ ] Domínios suspeitos
- [ ] Padrões de beacon (comunicação periódica)

DNS Tunneling:
- [ ] DNS queries com payloads grandes
- [ ] Queries para subdomínios anormais
- [ ] Muitas queries para mesmo domínio
```

**Semanas:** 10-12 (prático)  
**Tempo:** ~12h

---

### **Ferramentas Essenciais**
```
Reconhecimento:
- [ ] Nmap: port scanning, OS detection
- [ ] Whois: informações de domínio
- [ ] DNS tools: dig, nslookup, dnsenum
- [ ] Shodan: buscar dispositivos IoT expostos
- [ ] Google Dorking: encontrar informações sensíveis

Web Testing:
- [ ] Burp Suite Community (proxy, scanner)
- [ ] OWASP ZAP (alternativa open-source)
- [ ] curl: testes manuais
- [ ] wget: download de arquivos

Vulnerability Scanning:
- [ ] OpenVAS: scanner de vulnerabilidades
- [ ] Nessus (freemium): scan profissional
- [ ] Nuclei: detecção rápida de vulns

Exploitation:
- [ ] Metasploit: framework de exploitation
- [ ] SQLMap: automação de SQL injection
- [ ] Hydra: brute force

Network Analysis:
- [ ] Wireshark (já estudado)
- [ ] tcpdump: captura de CLI
- [ ] Zeek (NSM - Network Security Monitoring)

Password Testing:
- [ ] John the Ripper: quebra de hashes
- [ ] Hashcat: GPU-based cracking
- [ ] Rockyou.txt: wordlist comum
```

**Semanas:** 8-14 (prático)  
**Tempo:** ~15h

---

# FASE 3: AVANÇADO - Análise Profissional (Semanas 15-20)

*6 semanas para:*
- Análise de tráfego PROFISSIONAL
- Detecção de anomalias reais
- Projeto Major: Network Analyzer + Malware Analysis Framework
- Security+ 9-10 (Incident Response, Disaster Recovery)
- Bug Bounty: 1-2 primeiras tentativas

---

### **Análise Profissional de Tráfego**
```
Captura Estratégica:
- [ ] Definir perímetro de rede
- [ ] Capturar perímetro 24/7 com rotação de arquivos
- [ ] Filtrar tráfego importante
- [ ] Armazenar em repositório central

Análise:
- [ ] Baselines: tráfego "normal"
- [ ] Desvios: tráfego suspeito
- [ ] Timeline: quando anomalias começam
- [ ] Correlação: relacionar eventos

Relatórios:
- [ ] Documentar achados
- [ ] Impacto: confidencialidade, integridade, disponibilidade
- [ ] Recomendações: ações corretivas
- [ ] Evidências: PCAPs, screenshots
```

**Semanas:** 15-20 (prático em projetos)  
**Tempo:** ~20h

---

### **Projeto Major - Network Analyzer**
```
Funcionalidades:
- [ ] Capturar tráfego com Scapy/PyShark
- [ ] Análise em tempo real de pacotes
- [ ] Detecção de port scans
- [ ] Detecção de brute force
- [ ] Alertas de anomalias
- [ ] Relatórios em HTML/PDF

Stack Sugerido:
- [ ] Python + Flask (web interface)
- [ ] Scapy/PyShark (análise)
- [ ] SQLite (armazenamento)
- [ ] Matplotlib (gráficos)

Publicar em GitHub com:
- [ ] README profissional
- [ ] Documentação de instalação
- [ ] Exemplos de uso
```

**Semanas:** 15-20 (projeto integrado)  
**Tempo:** ~30h

---

# FASE 4: CAPSTONE - Portfolio Final (Semanas 21-26)

*6 semanas para consolidação, entrevistas, bug bounty*

---

## 🎓 Resumo de Recursos - 6 Meses

| Recurso | Semanas | Total Horas | Objetivo |
|---------|---------|-------------|----------|
| **Computação Básica** | PRÉ | 5-6 | Fundação |
| **Linux (LabEx)** | 1-6 | 49 | Proficiência básica |
| **Python** | 1-12 | 60 | Intermediário + Scripts |
| **Redes** | 1-8 | 64 | Profundidade em protocolos |
| **Criptografia** | 4-6 | 34 | Fundamentos + aplicações |
| **Security+** | 1-18 | 50 | Certificação pronta |
| **Livro TCP/IP** | 1-20 | 25 | Expert em análise |
| **Wireshark** | 1-26 | 50 | Profissional |
| **TryHackMe** | 2-20 | 40 | Prático aplicado |
| **Ferramentas** | 8-20 | 30 | Domínio de tools |
| **Projetos** | 1-26 | 100 | Portfolio |
| **TOTAL** | | **~600 horas** | **Expert Junior** |

---

## ✅ Checklist Final - 6 Meses

### Conhecimento
```
Computação Básica:
- [ ] Como computador funciona
- [ ] Binário, hex, decimal
- [ ] CPU, GPU, RAM, HD/SSD
- [ ] x86 vs x64 vs ARM

Linux (49h):
- [ ] 100+ comandos
- [ ] Permissões, usuários, grupos
- [ ] Processos, logs, serviços
- [ ] Scripts bash, cron jobs
- [ ] Privilege escalation basics

Redes (64h):
- [ ] OSI Model 7 camadas
- [ ] TCP/IP stack
- [ ] 20+ protocolos (TCP, UDP, DNS, HTTP, HTTPS, SSH, FTP, ARP, ICMP, DHCP)
- [ ] Sub-redes, CIDR, IPv4/IPv6
- [ ] Equipamentos: switch, router, firewall
- [ ] Wireshark: captura, filtros, análise

Python (60h):
- [ ] Fundamentos, estruturas de dados, funções
- [ ] File I/O, JSON, CSV
- [ ] Módulos: os, sys, json, datetime, requests
- [ ] Scapy basics (enviar pacotes)
- [ ] Automação de scripts
- [ ] 10+ projetos práticos

Criptografia (34h):
- [ ] Simétrica: AES, DES
- [ ] Assimétrica: RSA, ECC
- [ ] Hashing: SHA, MD5
- [ ] Certificados, PKI, TLS/SSL
- [ ] Aplicações práticas

Security (50h):
- [ ] CIA Triad
- [ ] OWASP Top 10 detalhado
- [ ] CVE, CWE, CVSS
- [ ] Vulnerability assessment
- [ ] Methodologies: PTES, OWASP WSTG

Wireshark (50h):
- [ ] Captura avançada
- [ ] Filtros complexos
- [ ] Análise de tráfego profissional
- [ ] Detecção de anomalias
- [ ] Relatórios e documentação

Ferramentas (30h):
- [ ] Nmap, Burp Suite, Metasploit
- [ ] SQLMap, Hydra, John the Ripper
- [ ] OpenVAS, Nessus, Nuclei
- [ ] tcpdump, Zeek basics
```

### Projetos
```
- [ ] News Bot (GitHub)
- [ ] Twitter/Discord Bot (GitHub)
- [ ] Network Analyzer (Python + Wireshark) (GitHub)
- [ ] Log Parser + Análise (GitHub)
- [ ] Brute Force Detector (Python + Scapy) (GitHub)
- [ ] 5+ scripts de segurança (GitHub)
```

### Publicações
```
- [ ] 15+ blog posts (Dev.to, Medium, Hashnode)
  - Tópicos: OSI model, TCP/IP, Wireshark, Criptografia, Python scripts, etc
- [ ] 5+ vídeos (YouTube/TikTok)
- [ ] 6+ projetos no GitHub com README profissional
- [ ] **1000+ LinkedIn followers**
```

### Certificações
```
- [ ] Security+: Teórico completo (agendar exam)
- [ ] Wireshark Certified Analyst: Conceitos (WCNA nivel 1)
```

### Pronto Para
```
- [ ] Entrevistas: SOC Analyst Junior ✓
- [ ] Entrevistas: Pentester Junior ✓
- [ ] Bug Bounty: Reports ativos
- [ ] HackTheBox: Máquinas Easy-Medium
- [ ] CTFs: Participação em competições
```

---

## 🚀 Próximas Etapas (Após 6 Meses)

- **OSCP Preparation** (4-6 meses)
- **SIEM Deep Dive** (Splunk, ELK)
- **Bug Bounty seriously** (10-15h/semana)
- **Certificações avançadas:** CEH, GIAC (GCIH, GSEC)
- **Malware Analysis Advanced**

---

## 🔧 Troubleshooting & Tips

### Se ficar atrasado:
```
Priorize:
1. Wireshark > 2. Security+ > 3. TryHackMe > 4. Projetos

Comprima se necessário, mas NÃO sacrifique profundidade.
```

### Se achar muito fácil:
```
Expanda:
- Mais rooms TryHackMe (HackTheBox começar)
- Projetos maiores e mais complexos
- Bug bounty (comece com recon)
```

### Se achar muito difícil:
```
Revise e desacelere:
- Estenda fase para 8-10 semanas
- Volte 1 semana anterior para rever
- Foque em 1 tópico por semana vs múltiplos
```

---

**Criado:** 17 de Janeiro de 2026  
**Versão:** 6 Meses COMPLETO (Expandido)  
**Status:** ✅ Pronto para Começar

---

**Desenvolvido especialmente com:**
- ✅ Computação Básica (fundação sólida)
- ✅ Linux checklist completo (49h)
- ✅ Redes checklist completo (64h)
- ✅ Python checklist completo (60h)
- ✅ Criptografia profunda (34h)
- ✅ Security checklist completo (50h)
- ✅ Profundidade (não superficial)
- ✅ Distribuição equilibrada (não massivo)
- ✅ Projetos reais + prático
- ✅ Publicações profissionais
- ✅ Pronto para entrevistas e bug bounty
