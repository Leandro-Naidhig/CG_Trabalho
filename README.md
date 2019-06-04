## Computação Gráfica

Este trabalho prático foi desenvolvido para a disciplina de Computação Gráfica, ministrada pelo professor Dr. Mário Liziér.

#### Integrantes: 

[Leandro Naidhig](https://github.com/Leandro-Naidhig/)

[Michele Argolo Carvalho](https://github.com/xmixele/)

#### Atividade Prática 1:
- Visualização de um modelo mais complexo;
- Utilização simples de shaders, apenas redimensionamento para o volume de visão.

#### Atividade Prática 2:
- Visualização de pelo menos dois objetos diferentes;


- Alguma iteração do usuário (teclado ou mouse), movendo pelo menos um dos objetos;



- Construção das matrizes na CPU para envio a GPU:

  Definimos o código umelemento renderizador , que no caso o utilizado é o WEBGL, em que o mesmo renderiza os objetos 


  renderer = new THREE.WebGLRenderer();
  renderer.render(scene, camera);

- Matriz de Transformação do modelo (uma diferente para cada modelo);


- Matriz de Visualização (uma para toda a a cena);

-> Para a Matriz de Visualização, referenciamos o objeto camera e aplicamos uma nova matriz que realiza a translação do objeto para a posição x=-50, y=0 e z=1200, de acordo com a linha de comando abaixo:

 camera.applyMatrix(new THREE.Matrix4().makeTranslation(-50, 0, 1200));

- Duas posições distintas de câmeras.

-> De acodo com a função "function key(e)" do código, permite o usuário visualizar a câmera em duas posições diferentes, clicando com o mouse as teclas 1 e 2 para mudar a posição da mesma. O comando camera.position.set() na função é responsável por mudar as coordenadas da câmera no cenário, em que os parâmetros do método correspondem as posições X, Y e Z.


