# Orbi.py
### Automatizador de PDOS - GNC/UFPI

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

Para usar o Orbi.py, você precisa ter **Python 3.x** instalado. As dependências externas são listadas no arquivo `requirements.txt`.

Para instalar as dependências, execute o seguinte comando:
```bash
pip install -r requirements.txt

```text
seu_projeto/
├── __init__.py
├── orbi.py
├── gui/
│   ├── __init__.py
│   ├── main_window.py
│   └── about_window.py
├── core/
│   ├── __init__.py
│   ├── pdos_processor.py
│   └── constants.py
└── assets/
    ├── gnc.png
    ├── ufpi.png
    └── qr_code.png
```
Certifique-se de que a pasta assets/ contém as imagens necessárias.
## ▶️ Executando o Programa

    Clone este repositório ou baixe os arquivos.

    Navegue até o diretório raiz do projeto (onde está o orbi.zip).
    Baixe a página e extraia.
    Dentro da pasta execute o programa com: 

python3 orbi.py

## 🧭 Passos na Interface Gráfica

Para usar o programa de forma eficiente, siga estes passos simples:

1.  **Selecione o Arquivo `.PDOS`**:
    * Clique no botão "Procurar..." e escolha o arquivo `.PDOS` gerado pelo seu cálculo.

2.  **Informe os Elementos**:
    * **Para projeção**: Digite os símbolos dos elementos separados por vírgula (ex: `C, O, Fe`).
    * **Para todos os elementos**: Digite `all` para processar automaticamente todos os elementos do arquivo.
    * **Para importar**: Use o botão "Carregar Elementos do FDF" para importar os símbolos diretamente de um arquivo `.fdf`.

3.  **Defina o Nome da Pasta de Saída**:
    * Digite o nome da pasta onde os arquivos `.dat` serão salvos.

4.  **Escolha a Ação**:
    * Clique em "Extrair PDOS Projetado" para gerar arquivos separados por orbital para cada elemento.
    * Clique em "Extrair TDOS" para gerar um único arquivo `TOTAL_DOS.dat`.

5.  **Verifique o Log**:
    * A área de log exibirá o status do processamento, incluindo avisos e mensagens de erro.

## 🛠️ Desenvolvimento

Este projeto foi desenvolvido em Python 3.x e utiliza:

    tkinter: Criação da interface gráfica

    Pillow: Manipulação de imagens

    os, re: Manipulação de arquivos e expressões regulares

## 🤝 Contribuições

Contribuições são bem-vindas!
Sinta-se à vontade para abrir uma issue ou enviar um pull request com sugestões, correções ou novas funcionalidades.

## ⚖️ Licença

Distribuído sob a [Licença MIT](https://opensource.org/licenses/MIT). Veja o arquivo `LICENSE` para mais detalhes.

## 👨‍🔬 Sobre

Este software é um trabalho acadêmico desenvolvido por:

Henrique Lago Liberato
Aluno de Física do ICV - UFPI
Membro do Grupo de Nanofísica Computacional (GNC) <br>
Orientador: Prof. Dr. Ramon Sampaio F.

📧 Contato: henrique.liberato@ufpi.edu.br

🔗 Conheça o GNC escaneando o QR Code abaixo:  
<img src="https://github.com/HenriqueDFT/Orbi.py/blob/main/qr(1)(1).png?raw=true" alt="QR Code GNC" width="200"/>
