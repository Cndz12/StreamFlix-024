# StreamFlix — Testes Automatizados com xUnit

Projeto desenvolvido para praticar testes automatizados e validar regras de negócio de uma plataforma fictícia de streaming, utilizando o ecossistema .NET e o framework xUnit.

## Sobre o projeto

O StreamFlix simula regras de negócio comuns em serviços de streaming, incluindo classificação de planos, cálculo de mensalidades com descontos e controle de acesso a conteúdos por idade.

O projeto tem como foco o desenvolvimento de testes automatizados para verificar o comportamento esperado das regras de negócio e identificar possíveis falhas na aplicação.

## Funcionalidades

- **Classificação de planos:** definição do plano de streaming com base na quantidade de telas simultâneas.
- **Descontos por período de contratação:** cálculo da mensalidade conforme o tempo de assinatura.
- **Controle de acesso a conteúdo:** validação de idade mínima e configurações de controle parental.
- **Testes automatizados:** estrutura dedicada à validação das regras de negócio.

## Regras de negócio

| Regra | Comportamento esperado |
|---|---|
| Plano Premium | 4 ou mais telas simultâneas |
| Plano Padrão | 2 telas simultâneas |
| Plano Básico | Demais quantidades de telas |
| Desconto anual | 20% para contratos de 12 meses ou mais |
| Desconto semestral | 10% para contratos de 6 a 11 meses |
| Sem desconto | Contratos inferiores a 6 meses |
| Conteúdo adulto | Permitido a partir dos 18 anos, desde que o controle parental não esteja ativo |

## Tecnologias utilizadas

- **C# / .NET** — desenvolvimento da aplicação.
- **xUnit** — framework para testes automatizados.
- **Python** — implementação complementar de regras de negócio.
- **Visual Studio / Visual Studio Code** — ambientes de desenvolvimento compatíveis.

## Estrutura do projeto

```text
streaming-flix-xunit/
├── StreamingFlix.App/
├── StreamingFlix.Tests/
├── PlanoStreamingService.py
├── StreamingFlix.sln
├── LICENSE
└── README.md
```

- `StreamingFlix.App`: projeto principal da aplicação.
- `StreamingFlix.Tests`: projeto dedicado aos testes automatizados.
- `PlanoStreamingService.py`: implementação em Python de regras relacionadas aos planos de streaming.
- `StreamingFlix.sln`: arquivo de solução .NET.

## Como executar os testes

### Pré-requisitos

- SDK do .NET compatível com a solução.
- Git instalado.

### 1. Clone o repositório

```bash
git clone https://github.com/Cndz12/streaming-flix-xunit.git
```

### 2. Acesse a pasta do projeto

```bash
cd streaming-flix-xunit
```

### 3. Execute os testes

```bash
dotnet test StreamingFlix.sln
```

O comando executa os testes configurados na solução e apresenta os resultados no terminal.

## Objetivos de aprendizagem

Este projeto permite praticar conceitos importantes de desenvolvimento de software, como:

- Testes unitários e validação de regras de negócio.
- Organização de projetos em soluções .NET.
- Uso do xUnit para automatizar verificações.
- Identificação de cenários válidos e inválidos.
- Aplicação de descontos e validação de condições de acesso.

## Licença

Este projeto está disponibilizado sob a licença MIT. Consulte o arquivo [LICENSE](LICENSE) para conhecer os termos de utilização.
