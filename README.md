# Strigoi — Downloads

Este repositório público contém somente os artefatos oficiais de distribuição do Strigoi.

## Download

Baixe a versão mais recente pela página de [Releases](https://github.com/jpgalvao-architect/strigoi-downloads/releases/latest). A versão atual é o instalador Windows x64 **Strigoi 0.1.16**.

## Nesta versão

### 0.1.16

- resolução compartilhada de caminhos entre anexos e ferramentas: relativos, prefixados pelo workspace, absolutos Windows e URIs file://;
- leitura de DOCX e outros documentos Office também pela ferramenta getFileContent, não apenas pelo anexo;
- arquivos externos anexados podem ser consultados na solicitação correspondente, sem abrir acesso irrestrito ao disco;
- skills e arquivos de apoio na pasta pessoal .agents/skills usam o diretório do usuário atual; carregamento aguarda a descoberta e informa o caminho real da skill;
- comparação de caminhos e listagens corrigida para diferenças de maiúsculas/minúsculas do Windows; raízes consultadas ao vivo;
- erros incluem caminho solicitado e URI resolvida, sem substituição silenciosa por README;
- validação automatizada com arquivos reais, incluindo leitura idêntica de DOCX por quatro formas de caminho. Isso não garante a qualidade do planejamento produzido por cada modelo local.

### 0.1.15

- o conteúdo extraído de documentos anexados acompanha a mensagem enviada ao modelo, inclusive no modo Planejar;
- o Strigoi usa o documento anexado como fonte e só pede que o usuário cole o texto se a extração falhar;
- anexos de arquivo são removidos do campo após o envio para evitar reutilização acidental; a mensagem já enviada permanece intacta.

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
