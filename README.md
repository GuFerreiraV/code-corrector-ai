# CodeCorrectorAI

O CodeCorrectorAI é uma ferramenta inteligente desenvolvida para auxiliar desenvolvedores na análise, correção e otimização de código-fonte. Utilizando o poder dos modelos de IA generativa do Google Gemini, a aplicação oferece uma revisão detalhada que vai além de simples correções sintáticas, abordando também lógica e boas práticas de programação.

## Funcionalidades

- **Correção Automática**: Identifica e corrige erros de sintaxe, indentação e lógica de programação.
- **Análise Técnica Detalhada**: Fornece uma explicação minuciosa dividida em:
    - **Erros de Lógica**: Explicação do bug e da solução.
    - **Erros de Sintaxe**: Correções estruturais.
    - **Boas Práticas**: Sugestões de refatoração seguindo padrões de mercado.
- **Exportação em Markdown**: Permite baixar o resultado da análise em um arquivo `.md` para fácil compartilhamento e documentação.
- **Suporte Multilinguagem**: Capaz de analisar diversas linguagens de programação reconhecidas pela IA.

## Tecnologias Utilizadas

- **Backend**: ASP.NET Core 10.0 (Razor Pages)
- **IA**: Google Gemini API (Modelo gemini-2.5-flash)
- **Frontend**: Bootstrap & CSS Customizado

## Configuração e Instalação

### Pré-requisitos
- [.NET 10.0 SDK](https://dotnet.microsoft.com/download/dotnet/10.0)
- Chave de API do Google Gemini (Obtenha em [Google AI Studio](https://aistudio.google.com/))

### Passos para Configuração

1. Clone o repositório:
   ```bash
   git clone <url-do-repositorio>
   cd CodeCorrectorAI
   ```

2. Configure sua Chave de API:
   No arquivo CodeCorrectorAI/appsettings.json (ou appsettings.Development.json), adicione sua chave:
   ```json
   {
     "Gemini": {
       "ApiKey": "SUA_CHAVE_AQUI"
     }
   }
   ```
   *Alternativamente, você pode definir uma variável de ambiente Gemini__ApiKey.*

3. Restaure as dependências e compile o projeto:
   ```bash
   dotnet build CodeCorrectorAI/CodeCorrectorAI.csproj
   ```

4. Execute a aplicação:
   ```bash
   dotnet run --project CodeCorrectorAI/CodeCorrectorAI.csproj
   ```
   Acesse em: http://localhost:5288

## Melhorias Futuras

- [ ] Persistência de histórico de análises em banco de dados (SQLite/SQL Server).
- [ ] Implementação de sistema de autenticação de usuários.
- [ ] Suporte a múltiplos modelos de IA para comparação de resultados.
- [ ] Interface dark mode otimizada para desenvolvedores.

---
Desenvolvido com foco na qualidade de código e aprendizado contínuo.
