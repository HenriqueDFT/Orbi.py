# Automatizador de PDOS - GNC/UFPI

---

Este é um programa desktop desenvolvido em **Python** com `Tkinter` e `Pillow` para automatizar o processamento de arquivos de Densidade de Estados (DOS) obtidos a partir de cálculos de **DFT (Teoria do Funcional da Densidade)**, com foco em projeções de Densidade de Estados Parcial (PDOS) e Densidade de Estados Total (TDOS). Ele foi criado com o intuito de facilitar a análise de dados computacionais para pesquisas em nanociência e materiais, no contexto acadêmico do **Grupo de Nanofísica Computacional (GNC)** da **Universidade Federal do Piauí (UFPI)**.

## 🌟 Recursos

* **Extração de PDOS Projetado**: Projeta a Densidade de Estados para orbitais de valência específicos de diferentes elementos químicos (s, p, d, f).
* **Extração de TDOS**: Calcula e salva a Densidade de Estados Total do sistema.
* **Seleção Flexível de Elementos**: Permite a seleção manual de elementos ou a opção de processar "todos" os elementos conhecidos pelo programa.
* **Leitura de Arquivos FDF**: Capacidade de carregar automaticamente os símbolos dos elementos presentes em um arquivo `.fdf` (formato de arquivo de entrada do SIESTA/TranSiesta).
* **Interface Gráfica Intuitiva (GUI)**: Desenvolvido com `Tkinter` para uma experiência de usuário amigável.
* **Log Detalhado**: Exibe o progresso e possíveis avisos/erros durante o processamento.
* **Organização de Saída**: Salva os resultados em uma pasta dedicada, nomeada pelo usuário, para fácil organização.

## 🚀 Como Usar

### Pré-requisitos

Certifique-se de ter o **Python 3** instalado em seu sistema. Além disso, você precisará instalar a biblioteca `Pillow` para o tratamento de imagens na interface gráfica:

```bash
pip install Pillow

Estrutura do Projeto

O programa espera a seguinte estrutura de arquivos:

seu_projeto/
├── __init__.py
├── main_app.py
├── gui/
│   ├── __init__.py
│   ├── main_window.py
│   └── about_window.py
├── core/
│   ├── __init__.py
│   ├── pdos_processor.py
│   └── constants.py
└── assets/
    ├── gnc(1).png
    ├── ufpi.png
    └── qr(1)(1).png

Certifique-se de que a pasta assets/ existe e contém as imagens necessárias.

Executando o Programa

    Clone este repositório ou baixe os arquivos para o seu computador.

    Navegue até o diretório raiz do projeto (onde o main_app.py está localizado) em seu terminal.

    Execute o programa com o seguinte comando:
    Bash

    python main_app.py

Passos na Interface Gráfica

    Selecione o Arquivo PDOS: Clique em "Procurar..." para escolher o arquivo de entrada (.PDOS) gerado pelo seu cálculo de DFT.

    Informe os Elementos:

        Para PDOS Projetado: Digite os símbolos dos elementos separados por vírgula (ex: C,O,Fe). Você também pode digitar all para processar todos os elementos listados no banco de dados interno.

        Carregar do FDF: Opcionalmente, clique em "Carregar Elementos do FDF" e selecione um arquivo .fdf do seu cálculo. O programa tentará extrair os símbolos dos elementos e preencher o campo "Elementos" automaticamente.

    Nome da Pasta de Saída: Defina um nome para a pasta onde os resultados (.dat) serão salvos.

    Escolha a Ação:

        Clique em "Extrair PDOS Projetado" para gerar arquivos .dat para cada orbital de valência dos elementos selecionados.

        Clique em "Extrair TDOS" para gerar um único arquivo TOTAL_DOS.dat contendo a densidade de estados total.

    Verifique o Log: A área de "Log de Processamento" exibirá o status da operação, avisos e erros.

🛠️ Desenvolvimento

Este projeto foi desenvolvido em Python 3.x e utiliza as seguintes bibliotecas:

    tkinter: Para a criação da interface gráfica.

    Pillow (PIL): Para o carregamento e manipulação de imagens (logotipos, QR Code).

    os e re: Para operações de sistema de arquivos e expressões regulares no processamento de texto.

🤝 Contribuições

Contribuições são bem-vindas! Se você tiver sugestões, encontrar bugs ou quiser implementar novas funcionalidades, sinta-se à vontade para abrir uma issue ou enviar um pull request.

👨‍🔬 Sobre

Este software é um trabalho acadêmico desenvolvido por Henrique Lago Liberato, aluno do curso de Física do Instituto de Ciências da Natureza, Meio Ambiente e Tecnologia (ICV) da Universidade Federal do Piauí (UFPI) e membro do Grupo de Nanofísica Computacional (GNC).

Orientador: Prof. Dr. Ramon Sampaio F.

Contato: henrique.liberato@ufpi.edu.br
