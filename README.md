<div>
        <img src="HPC LOGO.png" style="width: 500px; height:500px; margin-right: 20px;" />
</div>

# HPC reconstrói imagens com Algoritmos Genéticos
**Grupo:** HPC: High Phofocas & Condiments
<br>
**Integrantes:** Alice Barbarino Santos, Bruno Ferreira Brischi e Maria Eduarda de Oliveira Crist
<br>
**Instituição:** Ilum - Escola de ciência
<br>
## Apresentação
Este GitHub compõe um dos dois trabalhos finais de _Redes Neurais e Algoritmos Genéticos_, disciplina ministrada por Daniel Roberto Cassar na [Ilum - Escola de Ciências](https://ilum.cnpem.br). Dessa forma, esse projeto busca reconstruir imagens usando uma implementação de Algoritmos Genéticos com python. 

## Estrutura do Repositório
- _GA reconstruidor.ipynb_: Jupyter Notebook que apresenta o algoritmo genético e sua implementação.
- _image_test.py_: classe da referência [1] para criar e manipular imagens.
- _elitism_callback.py_: classe da referência [1] para modificar a função `eaSimple` da `deap`, implementando elitismo e _callback_.
- _Mona_Lisa_head.png_: imagem que será usada como teste do algoritmo genético.
- _HPC_logo_: Logo da equipe para exibi-lá no github e no notebook.
- _images_: diretório que contém os resultados do algoritmo a cada 100 gerações.
  

## Motivação
Algoritmos genéticos são ferramentas poderosas inspirados na biologia e que auxiliam na resolução de problemas de otimização, sendo muito populares pela sua capacidade de evoluirem e conseguirem soluções melhores com o decorrer do tempo, sendo uma alternativa aos métodos de otimização por busca em grade e busca aleatória [3][4]. Assim, a reconstrução de imagens é um método importante em processamento de imagem, já que pode ser aplicada em recuperar imagens corrompidas e em redução de ruído [2]. Então, propomos com esse projeto fazer uma implementação do algoritmo proposto pelos autores da referência [1], mas tentando realizar mudanças para melhorar a convergência da solução e aperfeiçoá-lo.

## Requisitos
É necessário o python instalado, além do Jupyter habilitado com as bibliotecas: `PIL`, `skimage`, `deap`, `IPython`, `cv2` (OpenCV), `matplotlib`, `numpy` e `random`, que são usadas em momentos variados do código.

## Bibliotecas
As principais bibliotecas utilizadas nesse trabalho são: 
- `PIL` para criar imagens e "desenhar" polígonos nela.
- `skimage` para computar o SSIM (uma das funções de fitness) e processar imagens.
- `cv2` para usar _color maps_ RGB na imagem criada.
- `matplotlib` para _plotar_ as imagens e gráficos de resultado.
- `deap` para construir e implementar todo o algoritmo genético.
- `IPython` para visualização de imagem em formato PIL.
- `random` para gerar valores aleatórios.

## Como utilizar
Nesse repositório, o usuário tem acesso à um notebook executável, que pode ser baixado e executado pelo usuário, com o intuito de que ele entenda passo a passo da construção do algoritmo genético, além de acompanhar sua evolução. Por já apresentar a rede neural treinada, o usuário pode usufruir desse notebook para fazer previsões por si só, desfrutando do modelo apresentado.

Obs.: o notebook foi executado em um Lenovo ThinkPad E14 i5, demorando algumas horas para sua execução completa; devido ao fato de ser um código pesado, recomendamos seu uso em uma máquina com um bom processador.

## Referências
[1] Wirsansky, E. (2020). Hands-on genetic algorithms with Python: applying genetic algorithms to solve real-world deep learning and artificial intelligence problems. Packt Publishing Ltd.

[2] Mirjalili, S., Song Dong, J., Sadiq, A. S., & Faris, H. (2020). Genetic algorithm: Theory, literature review, and application in image reconstruction. Nature-inspired optimizers: Theories, literature reviews and applications, 69-85.

[3] Notebok 1.3 e 1.5 da disciplina de Algoritmos Genéticos, de autoria do professor.

[4] Notebook 2.3 da disciplina de Algoritmos Genéticos, de autoria do professor.

