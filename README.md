# PlataformaAloca-o

# Plataforma de Gerenciamento e Alocação de Funcionários no Centro de Triagem de Logística

## Faculdade de Computação e Informática  
**Curso:** Ciência da Computação  
**Disciplina:** Engenharia de Software  

### Equipe
- Gustavo Fugulin Soares da Silva - 10418552  
- Otto Martins Mota - 10418170  
- Yuri Milliet da Silva - 10417884  

**São Paulo, 01/2025**

---

## Sumário

1. [Contexto de Negócio e Processos](#contexto-de-negocio-e-processos)
   - [Modelo de Negócio](#modelo-de-negocio)
   - [Diagrama de Classes de Domínio](#diagrama-de-classes-de-dominio)
2. [Casos de Uso e Requisitos](#casos-de-uso-e-requisitos)
   - [Diagrama de Casos de Uso](#diagrama-de-casos-de-uso)
   - [Diagrama de Estados](#diagrama-de-estados)
   - [Protótipo](#prototipo)
   - [Requisitos Funcionais](#requisitos-funcionais)
   - [Requisitos Não Funcionais](#requisitos-nao-funcionais)
3. [Modelos de Projeto](#modelos-de-projeto)
4. [Modelos de Componentes](#modelos-de-componentes)
5. [Modelo de Implantação](#modelo-de-implantacao)

---

## 1. Objetivo
O objetivo deste projeto é desenvolver uma plataforma de gerenciamento e alocação de funcionários para um centro de triagem logística. O sistema permitirá a alocação eficiente de funcionários com base na demanda, disponibilidade e qualificação, otimizando os processos internos e aumentando a produtividade.

### 1.1 Necessidade de Negócio
Atualmente, a alocação de funcionários é realizada de forma manual ou por planilhas, causando ineficiências como:

- Superalocação ou subalocação de funcionários.
- Falta de visibilidade sobre disponibilidade e qualificação.
- Dificuldade na gestão de turnos e escalas.
- Impacto negativo na produtividade e no tempo de processamento de mercadorias.

O sistema proposto visa solucionar essas deficiências por meio de automação e distribuição otimizada da equipe.

### 1.2 Visão Atual do Negócio
Atualmente, a gestão da alocação de funcionários ocorre da seguinte forma:
1. O supervisor analisa manualmente a demanda do centro de triagem.
2. A distribuição dos funcionários é feita sem critérios otimizados.
3. Mudanças de turno ocorrem sem planejamento adequado.
4. O registro de horas trabalhadas é manual e propenso a erros.

![image](https://github.com/user-attachments/assets/7e4092bc-c2f8-4f67-a487-6297042f530c)

Imagem 1: Diagrama BPMN “As is”



---

## 2. Contexto de Negócio e Processos
A nova solução busca automatizar a distribuição dos recursos humanos com base na demanda operacional e disponibilidade dos funcionários. 

### Análise SWOT
| **Fator** | **Descrição** |
|---|---|
| **Forças** | Automação da alocação, melhor gerenciamento de escalas, redução de erros humanos. |
| **Fraquezas** | Necessidade de treinamento inicial, resistência à mudança por parte dos supervisores. |
| **Oportunidades** | Aumento da produtividade, melhor integração com outros sistemas logísticos, possibilidade de expansão. |
| **Ameaças** | Dependência de infraestrutura digital, possíveis falhas no algoritmo de alocação. |

### 2.1 Modelo de Negócio Proposto
Com a implantação da plataforma, o fluxo de trabalho será otimizado:
1. O sistema analisará automaticamente a demanda e funcionários disponíveis.
2. Um algoritmo sugerirá a alocação ideal.
3. Os supervisores poderão ajustar e confirmar as sugestões.
4. A escala de trabalho será gerenciada digitalmente.
5. Os funcionários receberão notificações automáticas sobre suas alocações.

![image](https://github.com/user-attachments/assets/8020a32d-a1aa-4951-9e4d-2de6bbffebfe)

Imagem 2: Diagrama BPMN “To be”


### 2.2 Diagrama de Classes de Domínio

![image](https://github.com/user-attachments/assets/4f6feec8-fbea-41dd-8586-e16f11faf16f)

Imagem 3: Diagrama de Classe e Domínio

| **Nome da Classe** | **Descrição** |
|---|---|
| **Supervisor** | Gerencia o sistema e as alocações. |
| **Funcionário** | Representa um trabalhador do centro de triagem, com cargo, qualificações e disponibilidade. |
| **Setor** | Define um setor dentro do centro de triagem com uma quantidade necessária de funcionários. |
| **Turno** | Representa um período de trabalho com início e fim definidos. |
| **Alocação** | Relaciona um funcionário a um setor e turno. |
| **Sistema** | Responsável pelo processamento das alocações e envio de notificações. |

---

## 3. Casos de Uso e Requisitos

### 3.1 Diagrama de Casos de Uso

*Inserir diagrama de casos de uso aqui.*

### 3.2 Especificação do Cenário de Caso de Uso

| **Atores** | **Pré-condições** | **Fluxo Básico** | **Fluxo Alternativo** | **Pós-condições** |
|---|---|---|---|---|
| Supervisor, Funcionário | O funcionário deve estar cadastrado no sistema. | O supervisor revisa a sugestão de alocação e aprova. | Caso necessário, o supervisor altera manualmente a alocação. | O funcionário é notificado sobre a nova escala. |

### 3.3 Diagrama de Estados

*Inserir diagrama de estados aqui.*

### 3.4 Protótipo

*Inserir protótipo aqui.*

### 3.5 Requisitos Funcionais

| **ID** | **Descrição** |
|---|---|
| RF1 | O sistema deve permitir o cadastro de funcionários. |
| RF2 | O sistema deve permitir a alocação automática de funcionários. |
| RF3 | O sistema deve enviar notificações automáticas sobre mudanças na escala. |

### 3.6 Requisitos Não Funcionais

| **ID** | **Descrição** | **Classificação** |
|---|---|---|
| RNF1 | O sistema deve ser acessível via web e dispositivos móveis. | Essencial |
| RNF2 | O sistema deve possuir tempo de resposta inferior a 2 segundos. | Alto |

---

## 4. Modelos de Projeto
*Inserir diagramas de sequência e classes aqui.*

## 5. Modelos de Componentes
*Inserir diagramas de componentes aqui.*

## 6. Arquitetura em Camadas
*Descrever a divisão em camadas lógicas do sistema.*

## 7. Modelo de Implantação
*Elaborar um diagrama de deployment para o projeto.*
