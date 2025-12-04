# Relatório de Pentest: Desafio Final de Cibersegurança

![Status do Projeto](https://img.shields.io/badge/Status-Concluído-success)
![Foco](https://img.shields.io/badge/Foco-Pentesting-red)
![License](https://img.shields.io/badge/License-MIT-blue)

## Sobre o Projeto

Este repositório contém os artefatos e o relatório final desenvolvido como parte do **Desafio do Último Módulo do Curso de Cibersegurança da Kensei e Vai na Web**.

O objetivo principal foi atuar como um pentester (hacker ético), investigando um ambiente controlado (site-laboratório) para identificar vulnerabilidades, explorar falhas de segurança e propor mitigações, documentando todo o processo em um relatório técnico e executivo.

---

## Objetivos

- Realizar o reconhecimento (Information Gathering) do alvo designado.
- Identificar vetores de ataque e vulnerabilidades (CVEs, misconfigurations).
- Explorar falhas de segurança de forma controlada (Proof of Concept).
- Classificar a severidade dos riscos (CVSS).
- Elaborar um relatório profissional com recomendações de correção.
- Capturar flags espalhadas no laboratório.

## Ferramentas Utilizadas

Durante a análise, foram utilizadas as seguintes ferramentas e técnicas:

* **Sistema Operacional:** Kali Linux
* **Reconhecimento & Scanning:** Nmap, Nikto, Dirb
* **Análise Web:** Burp Suite, DevTools
* **Exploração:** Metasploit
* **Documentação:** Word

## Metodologia

A análise seguiu as fases padrão de um teste de intrusão:

1.  **Reconhecimento:** Mapeamento de portas, serviços e diretórios ocultos.
2.  **Análise de Vulnerabilidades:** Detecção de falhas conhecidas e configurações incorretas.
3.  **Exploração:** Tentativa de validar as vulnerabilidades encontradas (XSS, SQL Injection, Privilege escalation, etc.).
4.  **Pós-Exploração & Report:** Coleta de evidências e escrita do relatório.



## Resumo das Descobertas

> *Nota: Detalhes sensíveis foram sanitizados para este repositório público.*

O relatório completo aponta vulnerabilidades nas seguintes categorias (Exemplos):

- [x] **Crítica:** SQL Injection com Escalada de Privilégios
- [x] **Alta:** Possível vazamento de backup do banco de dados
- [x] **Média:** Cookie PHPSESSID sem HttpOnly
- [x] **Baixa:** Ausência de X-Frame-Options (Clickjacking)
