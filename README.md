# Strigoi — Downloads

Este repositório público contém somente os artefatos oficiais de distribuição do Strigoi.

## Download

Baixe a versão mais recente pela página de [Releases](https://github.com/jpgalvao-architect/strigoi-downloads/releases/latest). A versão atual é o instalador Windows x64 **Strigoi 0.1.14**.

## Nesta versão

### 0.1.14

- documentos podem ser arrastados do workspace ou de qualquer pasta local diretamente para o chat;
- extração de texto para DOCX, XLSX, PPTX, PDF, ODT e formatos de texto comuns;
- o anexo exato permanece como fonte; se ele não puder ser lido, o Strigoi mostra o problema em vez de escolher outro arquivo;
- modo Planejar usa ferramentas de leitura para consultar skills e o workspace sem editar arquivos ou executar comandos.

### 0.1.13

- corrigido o reconhecimento de prompts de planejamento combinados com anexos `#file:`;
- planejamento agora pode consultar skills e ler/pesquisar arquivos do workspace sem executar alterações ou comandos;
- localização de skills pessoais resolvida pelo diretório de usuário de cada instalação, incluindo `.agents/skills`;
- fluxo mais claro entre Planejar (checklist) e Agente (execução revisável).

### 0.1.12

- corrigida a listagem da pasta inicial de um workspace que possui regras em `.gitignore`;
- paths retornados pelas ferramentas são reutilizáveis, inclusive em projetos com espaços no nome;
- proteção contra ciclos de chamadas repetidas a ferramentas e orçamento ampliado para o agente;
- ao atingir o orçamento de ferramentas, o Strigoi produz uma resposta final em vez de encerrar a conversa com erro.

O código-fonte, a documentação interna e os arquivos de planejamento permanecem no repositório privado principal.
