# projeto-hemoansiedade\
**Projeto HemoAnsiedade — Protótipo de Software**\
**Software desenvolvido para fins acadêmicos e institucionais, sem registro formal de patente ou licença comercial vinculada.**\
**Objetivo:** Digitalizar e automatizar a aplicação do Inventário de Autoavaliação de Ansiedade para pacientes em tratamento de hemodiálise. 
A solução busca promover a inclusão digital de forma acessível e clinicamente relevante, 
com arquitetura preparada para futura integração aos sistemas institucionais do Ministério da Saúde.

**Idealização / Concepção:** Profa. Dra. Fabiana de Souza Orlandi\
**Desenvolvimento Low-Code (End-to-End) e UI/UX Design:** Rita de Cassia Zanetti Marchi\
**Instituição:** Universidade Federal de São Carlos (UFSCar)\
**Front-end / Interface:** Microsoft Power Apps\
**Linguagem de Fórmulas:** Power Fx\
**Microsoft Power Platform (Web, Android e iOS via Power Apps Mobile)**\
**Banco de Dados: Microsoft SharePoint (Listas Relacionais)**

**Status atual:** Pausado. No aguardo de etapas futuras (MVP funcional concluído)\
**Nível de validação:** 0 - O protótipo encontra-se totalmente funcional, realizando o fluxo completo de preenchimento, cálculo/processamento e gravação estruturada dos dados no banco de dados.\
**Testes realizados:** O protótipo funcional do aplicativo em andamento foi apresentado à idealizadora, obtendo avaliação positiva quanto à interface, usabilidade e aderência aos objetivos propostos.\
**Aviso de Uso Clínico:** Esta versão destina-se apenas à demonstração técnica e simulação de ambiente. O protótipo ainda não está liberado para aplicação direta com pacientes/usuários finais.\
**O código-fonte e os arquivos da aplicação encontram-se disponibilizados neste repositório no estágio atual de desenvolvimento para fins de registro, transparência e continuidade futura.**\
**Mês / Ano de desenvolvimento:** 05/2026 à 09/2026

**Notificação e Relatório Automatizado:** Ao acionar o comando de gravação, o sistema envia automaticamente uma cópia estruturada das respostas ao profissional de saúde responsável pela avaliação psicológica do paciente. O relatório transcreve cada questão, sua respectiva pontuação individual e o escore total obtido, permitindo identificar rapidamente os itens de maior impacto e fundamentar a definição de estratégias terapêuticas personalizadas.

**Abaixo, exemplo do e-mail gerado ao profissional de saúde:**
<details>
<summary><strong>📋 Clique aqui para visualizar a estrutura completa do e-mail </strong></summary>

**Título do e-mail:**  Autoavaliação de Ansiedade em Hemodiálise\
(Abaixo, corpo do e-mail)

Olá, segue Avaliação Final do Paciente: Nome do Paciente

1. Você sente dificuldade para se concentrar? = 3
2. Você se sente nervoso(a), ansioso(a) ou agitado(a) com facilidade? = 3
3. Você fica nervoso(a), com medo ou pavor de agulhas? = 2
4. Você fica nervoso(a), assustado(a) ou com medo da hemodiálise? = 3
5. Você se preocupa que a hemodiálise sobrecarregue a situação financeira da sua família? = 2
6. Você se preocupa que a hemodiálise afete suas atividades sociais? = 3
7. Você se sente preocupado(a) que a sua doença possa piorar a qualquer momento? = 2
8. Você sente sua mente inquieta (muitos pensamentos)? = 3
9. Você sente medo sem motivo? = 2
10. Você sente medo de perder o controle ou entrar em crise? = 3
11. Você sente muita dificuldade para relaxar? = 2
12. Você se sente impaciente e se estressa com os(as) outros(as) ao seu redor? = 3

Pontuação Total: 31

</details>

**Abaixo, estrutura do banco de dados sharepoints denominado: HemoAvaliacaoAnsiedade**
<details>
<summary><strong>📋 Clique aqui para visualizar a estrutura completa de campos do SharePoint (47 colunas)</strong></summary>


 
| Nome do Campo | Tipo do Campo |
| :--- | :--- |
| `Titulo` | Texto com uma linha |
| `NomePaciente` | Texto com uma linha |
| `DataNascimento` | Data e Hora |
| `Sexo` | Opção |
| `DataAvaliacao` | Data e Hora |
| `Pergunta1` | Texto com várias linhas |
| `Resposta1` | Número |
| `Pergunta2` | Texto com várias linhas |
| `Resposta2` | Número |
| `Pergunta3` | Texto com várias linhas |
| `Resposta3` | Número |
| `Pergunta4` | Texto com várias linhas |
| `Resposta4` | Número |
| `Pergunta5` | Texto com várias linhas |
| `Resposta5` | Número |
| `Pergunta6` | Texto com várias linhas |
| `Resposta6` | Número |
| `Pergunta7` | Texto com várias linhas |
| `Resposta7` | Número |
| `Pergunta8` | Texto com várias linhas |
| `Resposta8` | Número |
| `Pergunta9` | Texto com várias linhas |
| `Resposta9` | Número |
| `Pergunta10` | Texto com várias linhas |
| `Resposta10` | Número |
| `Pergunta11` | Texto com várias linhas |
| `Resposta11` | Número |
| `Pergunta12` | Texto com várias linhas |
| `Resposta12` | Número |
| `HoraAvaliacaoI` | Data e Hora |
| `HoraAvaliacaoF` | Data e Hora |
| `PontuacaoTotal` | Número |
| `Modificado` | Data e Hora |
| `Criado` | Data e Hora |
| `Criado por` | Pessoa ou Grupo |
| `Modificado por` | Pessoa ou Grupo |


**Nota**: As colunas Modificado, Criado, Criado por e Modificado por são campos padrão gerados automaticamente pelo sistema do SharePoint.
</details>


