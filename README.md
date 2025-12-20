# Projeto Pedagógico do Curso (PPC) - Engenharia Eletrônica UTFPR Toledo

## Descrição

Este repositório contém o Projeto Pedagógico do Curso (PPC) para o Curso de Engenharia Eletrônica da Universidade Tecnológica Federal do Paraná (UTFPR) - Campus Toledo. O documento foi desenvolvido seguindo as diretrizes do estilo ABNTEX2 e está estruturado conforme as normas da ABNT.

O Projeto Pedagógico do Curso é um documento fundamental que define a identidade do curso, seus objetivos, metodologias, estrutura curricular e diretrizes pedagógicas. Ele serve como referência para docentes, discentes e demais envolvidos no processo educativo.

## Autores e Contato

- **Autor:** Núcleo Docente Estruturante
- **Contato:** Prof. Felipe Walter Dafico Pfrimer - pfrimer@utfpr.edu.br
- **Última atualização:** 03/02/2021

## Estrutura do Projeto

```
ppc2021/
├── main.tex              # Arquivo principal do documento LaTeX
├── capa.tex              # Modelo de capa
├── dados_gerais.tex      # Informações gerais do curso
├── identificacao.tex     # Identificação do documento
├── comandos.tex          # Comandos personalizados
├── references.bib        # Referências bibliográficas
├── teste.tex             # Arquivo de teste (opcional)
├── main.pdf              # Versão compilada do documento (gerada automaticamente)
├── README.md             # Este arquivo
├── QWEN.md               # Documentação do projeto para Qwen Code
├── LICENSE               # Licença do projeto
├── .gitignore            # Arquivos ignorados pelo Git
├── Anexos/               # Pasta para anexos
├── Apendices/            # Pasta para apêndices
├── Caps/                 # Pasta com os capítulos do PPC
├── Contadores/           # Pasta com contadores de horas
└── ...
```

## Conteúdo dos Capítulos

O PPC está dividido em diversos capítulos que abordam diferentes aspectos do curso:

- **Capítulo 1:** Contextualização da Instituição
- **Capítulo 2:** Valores e Princípios Institucionais
- **Capítulo 3:** Políticas de Ensino
- **Capítulo 4:** Contextualização (do curso)
- **Capítulo 5:** Matriz Curricular
- **Capítulo 6:** (Conteúdo específico)
- **Capítulo 7:** Estrutura Organizacional do Curso
- **Capítulos 8-11:** (Conteúdos específicos adicionais)

## Requisitos para Compilação

Para compilar este documento LaTeX, você precisará de:

- Um sistema LaTeX completo (como TeX Live, MiKTeX ou MacTeX)
- Suporte para o pacote ABNTEX2
- Compilador pdfLaTeX ou XeLaTeX

## Compilação do Documento

### Opção 1: Compilação básica

```bash
# Compilar com pdfLaTeX
pdflatex main.tex
pdflatex main.tex  # segunda compilação para atualizar referências cruzadas
```

### Opção 2: Compilação completa com referências bibliográficas e nomenclatura

Para garantir que todas as referências, sumários, lista de nomenclatura e índices estejam corretamente atualizados:

```bash
pdflatex main.tex
bibtex main
makeindex main.nlo -s nomencl.ist -o main.nls
pdflatex main.tex
pdflatex main.tex
```

### Opção 3: Usando XeLaTeX

```bash
# Compilar com XeLaTeX
xelatex main.tex
bibtex main
makeindex main.nlo -s nomencl.ist -o main.nls
xelatex main.tex
xelatex main.tex
```

### Resultado da Compilação
Após a compilação bem-sucedida, o arquivo `main.pdf` será gerado. O documento completo contém aproximadamente 213 páginas.

### Aviso sobre Warnings
Durante a compilação, podem ocorrer alguns warnings de "overfull hbox" ou "underfull hbox". Estes são avisos comuns em documentos LaTeX e indicam que o texto pode estar levemente fora dos limites da página ou que o espaçamento não é ideal. Estes warnings não afetam a funcionalidade ou a qualidade geral do documento, apenas indicam que pequenos ajustes de layout poderiam ser feitos para uma tipografia perfeita.

### Opção 4: Usando um editor LaTeX

Você pode usar editores como TeXstudio, Overleaf, ou VS Code com extensões LaTeX para compilar o documento.

## Personalização

### Dados Gerais
Edite o arquivo `dados_gerais.tex` para inserir informações específicas do seu curso, como nome do curso, nomes dos coordenadores, datas, etc.

### Comandos Personalizados
Adicione comandos LaTeX personalizados no arquivo `comandos.tex` para facilitar a escrita do documento.

### Capítulos
Os capítulos estão organizados na pasta `Caps/`. Adicione ou modifique os arquivos `.tex` nesta pasta para alterar o conteúdo do PPC.

## Boas Práticas para Manutenção

1. **Versionamento:** Este repositório utiliza Git para controle de versão. Sempre faça commits com mensagens descritivas.

2. **Backups:** Mantenha cópias de segurança regulares do projeto.

3. **Documentação:** Atualize a documentação (como este README) quando fizer alterações significativas.

4. **Testes:** Sempre compile o documento após fazer alterações para verificar se não há erros.

5. **Colaboração:** Para trabalhos colaborativos, utilize branches separados e pull requests para revisão antes de mesclar alterações.

## Contribuição

Se você for membro do corpo docente ou administrativo e deseja contribuir com este PPC:

1. Faça um fork deste repositório
2. Crie uma branch para sua feature (`git checkout -b feature/NovaFeature`)
3. Faça commit de suas alterações (`git commit -m 'Adiciona nova seção'`)
4. Faça push para a branch (`git push origin feature/NovaFeature`)
5. Abra um Pull Request

## Licença

Este projeto está licenciado conforme os termos encontrados no arquivo `LICENSE`.

## Suporte

Para suporte técnico com o documento LaTeX, utilize os canais de suporte da comunidade ABNTEX2.

Para questões específicas sobre o conteúdo do PPC, entre em contato com o Núcleo Docente Estruturante do Curso de Engenharia Eletrônica da UTFPR Toledo.