Análise de Performance: Algoritmos de Ordenação em Python vs. C++

Este projeto foi desenvolvido para realizar uma análise comparativa de performance entre algoritmos de ordenação implementados nas linguagens Python e C++. A análise foca em duas métricas principais: tempo de execução e pico de uso de memória.

Descrição do Projeto

O objetivo é comparar a eficiência de um algoritmo de ordenação simples e ineficiente (Bubble Sort) com um algoritmo de ordenação otimizado e nativo de cada linguagem (Timsort do Python e Introsort do C++).

O script principal de análise (analise.py) orquestra a execução dos diferentes scripts de ordenação, coleta os dados de performance, calcula estatísticas (média e mediana) e gera gráficos comparativos para facilitar a visualização dos resultados.

Funcionalidades

Implementações em Python e C++: Contém códigos para ordenação de números em ambas as linguagens.

Dois Algoritmos por Linguagem:

bubble: Implementação do Bubble Sort.

efficient: Utiliza a função de ordenação padrão e otimizada da linguagem.

Análise Automatizada: O script analise.py executa cada versão do algoritmo múltiplas vezes para garantir uma medição consistente.

Coleta de Métricas: Mede o tempo de execução (em milissegundos) e o pico de uso de memória (em Kilobytes).

Visualização de Dados: Gera 4 gráficos de barras para comparar a média e a mediana do tempo e da memória entre as quatro implementações.

Relatório em Tabela: Exibe um resumo claro e formatado dos resultados no console.

Tecnologias Utilizadas

Python 3

matplotlib: Para a geração dos gráficos.

psutil: Para monitoramento de uso de memória do processo.

C++

Compilador g++ (ou similar, como Clang/MSVC).

Instalação e Configuração

Siga os passos abaixo para preparar o ambiente e rodar o projeto.

Pré-requisitos

Python 3 e pip instalados.

Um compilador C++, como o g++. (Para usuários de Windows, o MinGW ou o WSL são boas opções).

Passos para Instalação

Clone o Repositório

git clone <URL_DO_SEU_REPOSITORIO>
cd <NOME_DO_SEU_REPOSITORIO>


Instale as Dependências do Python
O projeto utiliza duas bibliotecas externas que precisam ser instaladas. Execute o comando abaixo no seu terminal:

pip install matplotlib psutil


Compile o Código C++
Navegue até o diretório do projeto e use um compilador C++ para criar o arquivo executável.

No Linux ou macOS:

g++ -o sorter_cpp sorter_cpp.cpp


No Windows:

g++ -o sorter_cpp.exe sorter_cpp.cpp


Isso criará um executável chamado sorter_cpp (ou sorter_cpp.exe) que será utilizado pelo script de análise.

Como Executar

Após a instalação e compilação, você pode executar a análise completa com um único comando.

Certifique-se de que o arquivo arq.txt está presente no mesmo diretório. Ele contém os números que serão ordenados.

Execute o script de análise principal:

python analise.py


O script irá:

Executar cada um dos quatro cenários (Python Bubble, Python Efficient, C++ Bubble, C++ Efficient) 10 vezes.

Imprimir o progresso no terminal.

Ao final, exibir uma tabela com a média e mediana dos resultados.

Salvar quatro imagens de gráficos (.png) no diretório do projeto com os resultados visuais.

Exibir os gráficos na tela.

Arquivos do Projeto

analise.py: O orquestrador principal. Executa os outros scripts, coleta e analisa os dados de performance, e gera os gráficos.

sorter_py.py: Contém as implementações dos algoritmos bubble_sort e efficient_sort em Python. Lê dados de arq.txt e escreve em arq-saida.txt.

sorter_cpp.cpp: Contém as implementações dos algoritmos bubble_sort e efficient_sort em C++. Também lê de arq.txt e escreve em arq-saida.txt.

arq.txt: Arquivo de entrada com a lista de números a serem ordenados.
