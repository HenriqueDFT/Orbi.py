# Automatizador de PDOS - GNC/UFPI

---

Este é um programa desktop desenvolvido em **Python**, utilizando `Tkinter` e `Pillow`, para automatizar o processamento de arquivos de Densidade de Estados (DOS) obtidos a partir de cálculos de **DFT (Teoria do Funcional da Densidade)**. O foco está na projeção da Densidade de Estados Parcial (PDOS) e na extração da Densidade de Estados Total (TDOS).  

O software foi criado com o intuito de facilitar a análise de dados computacionais em pesquisas de nanociência e ciência dos materiais, no contexto acadêmico do **Grupo de Nanofísica Computacional (GNC)** da **Universidade Federal do Piauí (UFPI)**.

---

## 🌟 Recursos

- **Extração de PDOS Projetado**: Projeta a densidade de estados para orbitais de valência específicos (s, p, d, f) de diferentes elementos químicos.  
- **Extração de TDOS**: Calcula e salva a densidade de estados total do sistema.  
- **Seleção Flexível de Elementos**: Permite selecionar elementos manualmente ou processar todos os disponíveis automaticamente.  
- **Leitura de Arquivos `.fdf`**: Carrega os símbolos dos elementos diretamente de arquivos de entrada do SIESTA/TranSiesta.  
- **Interface Gráfica Intuitiva (GUI)**: Desenvolvida com `Tkinter` para facilitar a experiência do usuário.  
- **Log Detalhado**: Acompanha o progresso, erros e alertas em tempo real.  
- **Organização de Saída**: Resultados são salvos em uma pasta nomeada pelo usuário para fácil organização.

---

## 🚀 Como Usar

### 📦 Pré-requisitos

- Python 3.x instalado  
- Instalar o `Pillow` com:


pip install Pillow

## 📁 Estrutura do Projeto
'''
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
'''
Certifique-se de que a pasta assets/ contém as imagens necessárias.
## ▶️ Executando o Programa

    Clone este repositório ou baixe os arquivos.

    Navegue até o diretório raiz do projeto (onde está o main_app.py).

    Execute o programa com:

python main_app.py

## 🧭 Passos na Interface Gráfica

    Selecionar Arquivo PDOS
    Clique em "Procurar..." e selecione o arquivo .PDOS gerado pelo seu cálculo.

    Informar os Elementos

        Para projeção: Digite os símbolos separados por vírgula (ex: C,O,Fe).

        Digite all para processar todos os elementos suportados.

        Ou use o botão "Carregar Elementos do FDF" para importar os símbolos a partir de um arquivo .fdf.

    Nome da Pasta de Saída
    Defina o nome da pasta onde os arquivos .dat serão salvos.

    Escolher Ação

        Clique em "Extrair PDOS Projetado" para gerar arquivos separados por orbital.

        Clique em "Extrair TDOS" para gerar um único arquivo TOTAL_DOS.dat.

    Verificar o Log
    A área de log exibirá o status, avisos e mensagens de erro.

## 🛠️ Desenvolvimento

Este projeto foi desenvolvido em Python 3.x e utiliza:

    tkinter: Criação da interface gráfica

    Pillow: Manipulação de imagens

    os, re: Manipulação de arquivos e expressões regulares

## 🤝 Contribuições

Contribuições são bem-vindas!
Sinta-se à vontade para abrir uma issue ou enviar um pull request com sugestões, correções ou novas funcionalidades.
## 👨‍🔬 Sobre

Este software é um trabalho acadêmico desenvolvido por:

Henrique Lago Liberato
Aluno de Física do ICV - UFPI
Membro do Grupo de Nanofísica Computacional (GNC)
Orientador: Prof. Dr. Ramon Sampaio F.

📧 Contato: henrique.liberato@ufpi.edu.br

🔗 Conheça o GNC escaneando o QR Code abaixo:
![qr(1)(1).png]()
