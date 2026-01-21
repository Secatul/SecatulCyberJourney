# 📚 Roadmap - Checklist Smart Notes
## SOC Analyst → Pentester Junior

**Data:** 17 de Janeiro - 17 de Julho 2026  
**Formato:** Smart Notes + Checklists  
**Total:** 134 tópicos | 5 Fases | ~600h  

---

## 📋 Como Usar Este Documento

- [ ] Imprima ou use digitalmente no Obsidian
- [ ] Marque ☑️ conforme completa cada tópico  
- [ ] ⭐ indica importância (⭐⭐⭐ = CRÍTICO)
- [ ] Atualize em seu GitHub/Obsidian regularmente
- [ ] Revise a cada semana: o que funcionou? O que não?

---

## PRÉ-ROADMAP: Fundações Essenciais

### Computação Básica

- [ ] **CPU, GPU, RAM, HD/SSD** ⭐⭐  
  → Componentes físicos que fazem o PC funcionar

- [ ] **Sistema Binário** ⭐⭐  
  → 0s e 1s: como computadores pensam

- [ ] **Software vs Hardware** ⭐  
  → Programas ↔ Componentes físicos

- [ ] **Como Funciona SO** ⭐⭐  
  → Gerenciador entre você e hardware

- [ ] **x86 vs x64 vs ARM** ⭐  
  → Arquiteturas: 32bits, 64bits, mobile

### Redes Basics

- [ ] **Internet Overview** ⭐  
  → ISP → Backbone → Sua rede

- [ ] **IP vs MAC** ⭐⭐⭐  
  → IP=lógico, MAC=físico (ambos necessários)

- [ ] **LAN vs WAN** ⭐⭐  
  → Local ↔ Mundo

- [ ] **Equipamentos Rede** ⭐⭐  
  → Router, Switch, Access Point, Firewall, Modem

- [ ] **Protocolos Preview** ⭐⭐⭐  
  → Regras de comunicação (HTTP, DNS, TCP, UDP)

### Terminologia Segurança

- [ ] **Segurança Informação** ⭐  
  → Proteger dados contra acesso não autorizado

- [ ] **CIA Triad** ⭐⭐⭐  
  → Confidentiality, Integrity, Availability

- [ ] **Vulnerabilidade vs Ameaça** ⭐⭐  
  → Fraqueza + Exploit = Risco

- [ ] **Exploit vs Payload** ⭐⭐  
  → Código que explora + o que entrega

- [ ] **White/Gray/Black Hat** ⭐⭐  
  → Ético, neutro, malicioso

- [ ] **OWASP Top 10** ⭐⭐⭐  
  → 10 vulnerabilidades web mais perigosas

- [ ] **CVE vs CWE vs CVSS** ⭐⭐  
  → ID vulnerabilidade, categoria, score (0-10)

---

## FASE 1: Fundações Sólidas (Semanas 1-6)

### Linux Essencial

- [ ] **Estrutura Diretórios** ⭐⭐⭐  
  → /, /home, /etc, /var, /tmp, /usr, /bin

- [ ] **Navegação** ⭐⭐⭐  
  → pwd, ls, cd, ls -la, cd ~

- [ ] **Arquivos** ⭐⭐⭐  
  → touch, mkdir, cp, mv, rm, rm -rf

- [ ] **Propriedade Arquivos** ⭐⭐⭐  
  → Ownership: user:group, chmod, chown

- [ ] **Permissões Octal** ⭐⭐⭐  
  → 755 (rwxr-xr-x), 644 (rw-r--r--), 777

- [ ] **Processos** ⭐⭐  
  → ps, ps aux, top, kill PID, nice, renice

- [ ] **Logs** ⭐⭐  
  → /var/log/, tail, grep, journalctl, syslog

- [ ] **Pacotes** ⭐⭐  
  → apt install, apt update, apt remove

- [ ] **Scripts Bash** ⭐⭐  
  → if, for, while, functions, pipes |, redirecionamento >

- [ ] **Cron Jobs** ⭐⭐  
  → Agendamento: crontab -e, automação

- [ ] **Systemd** ⭐⭐  
  → systemctl start/stop/enable/disable, services

### Redes TCP/IP

- [ ] **OSI Model** ⭐⭐⭐  
  → 7 camadas: Física, Link, Network, Transport, Session, Presentation, Application

- [ ] **TCP Protocol** ⭐⭐⭐  
  → Confiável, ordered, handshake 3-way (SYN, SYN-ACK, ACK)

- [ ] **UDP Protocol** ⭐⭐⭐  
  → Rápido, sem garantia, connectionless

- [ ] **IPv4 vs IPv6** ⭐⭐  
  → 32bits vs 128bits, notações diferentes

- [ ] **DNS** ⭐⭐⭐  
  → Traduz domain.com → 8.8.8.8, tipo A/AAAA/MX/CNAME

- [ ] **ICMP (Ping)** ⭐⭐  
  → Echo Request/Reply, diagnóstico

- [ ] **DHCP** ⭐⭐  
  → Atribui IP dinamicamente: DISCOVER → OFFER → REQUEST → ACK

- [ ] **ARP** ⭐⭐⭐  
  → IP → MAC mapping, arp spoofing risk

- [ ] **SSH** ⭐⭐⭐  
  → Acesso remoto seguro, porta 22

- [ ] **HTTP/HTTPS** ⭐⭐⭐  
  → Web protocol, porta 80/443, GET/POST/PUT/DELETE

- [ ] **TLS/SSL** ⭐⭐  
  → Criptografia da web, handshake, certificados

- [ ] **Sub-redes** ⭐⭐⭐  
  → CIDR notation (/24, /25), calcular ranges

- [ ] **Equipamentos** ⭐⭐  
  → Switch (L2), Router (L3), Firewall, AP WiFi

### Python Fundamentals

- [ ] **Variáveis & Tipos** ⭐⭐⭐  
  → int, float, str, bool, type()

- [ ] **Operadores** ⭐⭐⭐  
  → Aritméticos, comparação (==, !=, <, >), lógicos (and, or, not)

- [ ] **Strings** ⭐⭐⭐  
  → Concatenação, f-strings, slicing, split(), join()

- [ ] **Listas** ⭐⭐⭐  
  → append, remove, pop, slicing, list comprehension

- [ ] **Dicts** ⭐⭐  
  → key:value, .items(), .keys(), .values(), .get()

- [ ] **Tuples** ⭐⭐  
  → Imutáveis, unpacking x, y = tupla

- [ ] **Sets** ⭐⭐  
  → Únicos, union, intersection, difference

- [ ] **Controle** ⭐⭐⭐  
  → if/elif/else, for, while, break, continue

- [ ] **Funções** ⭐⭐⭐  
  → def, return, default params, *args, **kwargs

- [ ] **Imports** ⭐⭐  
  → import, from X import Y, built-ins: os, sys, json

- [ ] **File I/O** ⭐⭐  
  → open(), read(), write(), with statement

- [ ] **JSON** ⭐⭐  
  → json.load(), .dump(), .loads(), .dumps()

- [ ] **Tratamento Erros** ⭐⭐  
  → try/except/finally, raise, custom exceptions

- [ ] **Exercism** ⭐⭐⭐  
  → Resolver 15+ problemas progressivos

### Wireshark Basics

- [ ] **Captura** ⭐⭐⭐  
  → Interface selection, start/stop capture

- [ ] **Filtros** ⭐⭐⭐  
  → tcp, udp, icmp, dns, arp, tcp.port == 80

- [ ] **TCP Analysis** ⭐⭐⭐  
  → Ver 3-way handshake, flags (SYN, ACK, FIN, RST)

- [ ] **Seguir Stream** ⭐⭐  
  → Follow TCP Stream: ver conversa completa

- [ ] **DNS** ⭐⭐  
  → Query/Response, lookup type A/AAAA

- [ ] **ARP** ⭐⭐  
  → Request/Reply, local network mapping

- [ ] **Exportar** ⭐  
  → Save .pcap, exportar objetos HTTP

- [ ] **Estatísticas** ⭐⭐  
  → Endpoints, Conversations, Protocol Hierarchy

### Criptografia Intro

- [ ] **Simétrica** ⭐⭐  
  → AES, DES: mesma chave, rápida

- [ ] **Assimétrica** ⭐⭐  
  → RSA, ECC: pública+privada, lenta

- [ ] **Hashing** ⭐⭐⭐  
  → SHA-256, MD5: one-way, verificação integridade

- [ ] **Salt & Pepper** ⭐⭐  
  → Proteção contra rainbow tables

- [ ] **Certificados** ⭐⭐  
  → X.509, PKI, CA validation

---

## FASE 2: Intermediário (Semanas 7-14)

### Security+ Topics

- [ ] **Autenticação** ⭐⭐⭐  
  → Password, MFA, biométrica, token

- [ ] **Autorização** ⭐⭐  
  → Role-based, attribute-based access control

- [ ] **Risk Management** ⭐⭐  
  → Identificar, analisar, mitigar, monitorar

- [ ] **Threat Modeling** ⭐⭐  
  → Atacante, alvo, método, impacto

- [ ] **Incident Response** ⭐⭐⭐  
  → Identify, Contain, Eradicate, Recover, Lessons

- [ ] **Business Continuity** ⭐⭐  
  → Backup, disaster recovery, RTO/RPO

### OWASP Top 10

- [ ] **SQL Injection** ⭐⭐⭐  
  → WHERE 1=1, UNION based, detecção Wireshark

- [ ] **Broken Auth** ⭐⭐⭐  
  → Weak creds, session fixation, credential stuffing

- [ ] **Data Exposure** ⭐⭐⭐  
  → Texto claro HTTP, criptografia fraca, backups

- [ ] **XXE** ⭐⭐  
  → XML parser exploitation, file disclosure

- [ ] **Access Control** ⭐⭐⭐  
  → iDOR, horizontal vs vertical privilege escalation

- [ ] **Misconfiguration** ⭐⭐⭐  
  → Default creds, .git exposto, headers missing

- [ ] **XSS** ⭐⭐⭐  
  → Stored, Reflected, DOM - roubo de cookies/sessão

- [ ] **Deserialization** ⭐⭐  
  → RCE potencial em Java, Python, PHP

- [ ] **Known Vulns** ⭐⭐  
  → Dependências outdated, CVE tracking

- [ ] **Logging** ⭐  
  → Eventos críticos não logados, sem alertas

### Detecção Anomalias

- [ ] **Port Scans** ⭐⭐⭐  
  → SYN flood → muitos SYN, poucos SYN-ACK

- [ ] **Brute Force** ⭐⭐⭐  
  → Muitas tentativas TCP RST (auth rejeitada)

- [ ] **DDoS** ⭐⭐  
  → Tráfego massivo, mesma origem, Statistics

- [ ] **Data Exfiltration** ⭐⭐⭐  
  → Tráfego saindo >> entrando, IPs desconhecidos

- [ ] **Malware C&C** ⭐⭐  
  → Beacons periódicos, domínios suspeitos

- [ ] **DNS Tunneling** ⭐⭐  
  → DNS queries com payload grande, subdomínios

### Ferramentas

- [ ] **Nmap** ⭐⭐⭐  
  → Port scanning, OS detection, service version

- [ ] **Burp Suite** ⭐⭐⭐  
  → Web proxy, interceptação, scanning, repeater

- [ ] **Metasploit** ⭐⭐  
  → Framework exploitation, payloads

- [ ] **SQLMap** ⭐⭐  
  → Automação SQL injection

- [ ] **Hydra** ⭐⭐  
  → Brute force, múltiplos serviços

- [ ] **Wireshark Avançado** ⭐⭐⭐  
  → Filtros complexos, exportar dados, análise profissional

---

## FASE 3 & 4: Avançado + Capstone (Semanas 15-26)

### Análise Profissional

- [ ] **Captura Estratégica** ⭐⭐⭐  
  → Perímetro 24/7, rotação arquivos, repositório central

- [ ] **Baselines** ⭐⭐⭐  
  → Tráfego 'normal', desvios, timeline, correlação

- [ ] **Relatórios** ⭐⭐⭐  
  → Achados, impacto CIA, recomendações, PCAPs/screenshots

- [ ] **Investigação Forense** ⭐⭐  
  → Chain of custody, ferramentas, documentação

### Capstone & Portfolio

- [ ] **GitHub Projects** ⭐⭐⭐  
  → 6+ repos profissionais com READMEs

- [ ] **Blog Posts** ⭐⭐⭐  
  → 15+ artigos em Dev.to/Medium/Hashnode

- [ ] **Vídeos** ⭐⭐  
  → 5+ vídeos YouTube/TikTok

- [ ] **Network Analyzer** ⭐⭐⭐  
  → Projeto prático: detecção de anomalias

- [ ] **Bug Bounty** ⭐⭐⭐  
  → Recon, scanning, testing, relatórios

- [ ] **Entrevistas** ⭐⭐⭐  
  → SOC Analyst, Pentester Junior ready

---
