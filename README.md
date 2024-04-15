## Objectivo
A página fornecida é usada por um laboratório para fazer o registo de pesagens de filtros.

Cada filtro tem duas pesagens, uma inicial, e uma final. O resultado da pesagem do filtro é a diferença entre o peso final e o peso inicial.

Neste momento existem duas páginas iguais para registar o peso inicial e o final.

O objectivo do exercicio é alterar a página fornecida de forma a permitir fazer o registo de ambos os pesos num só sitio.



### Inputs
Todos estes inputs têm de ter a indicação das unidades de medida e são registados com duas casas decimais.

Para cada um dos dois pesos (inicial e final) o utilizador tem registar:
- 3 Leituras (leitura 1, leitura 2, e leitura 3) de peso em **mg**;
- Temperatura ambiente em **℃**;
- Humidade Relativa (HR) em **%**;
- Pressão atmosférica em **mbar**;

Além deste inputs tem de existir um campo único na página para registo de notas ou observações.



### Outputs
Para cada um dos dois pesos (inicial e final) indicar:
- Resultado extrapolado com indicação da incerteza, em **mg**;
- Validade da pesagem com indicação do critério de aceitação e da diferença de massa, em **mg**;

Deve também ser indicado em destaque o resultado do filtro (valor da diferença entre o peso final e o inicial) com a respectiva incerteza, em mg.

O critério de aceitação (CA) é fornecido pelo backend e guardado no respectivo hiddenfield (#Criterio).

Todos os outputs tem de ser atualizados automaticamente sempre que o utilizador introduz uma das leituras.

Os registos de temperatura, humidade, e pressão não têm influência nos resultados.

As funções e fórmulas de cálculo estão todas no código JS no fim da página.



### Funcionalidades
- Adicionar botões que permitam copiar todos os valores de um dos pesos para o outro;
- Bónus: adicionar botão para anular esta ação em caso de click acidental;



### Outras considerações e requisitos
- A aréa de cálculos intermédios pode ser removida;
- Os botões de guardar, cancelar, copiar, etc, têm de estar sempre visiveís;
- Ter em atenção a hierarquia visual da página, nomeadamente no que diz respeito ao destaque dado à ação principal (guardar), e às secundárias;
- Todas as ações devem usar verbos (guardar, cancelar) ou um icone. Caso seja usado um ícone deve ser colocada a descrição da ação no título do botão;
- Todos os inputs devem idealmente ser visiveis sem ser preciso fazer scroll vertical, sendo que os valores das 3 leituras são inputs principais, e os da temperatura, humidade, e pressão, inputs secundários;
- Usar sempre que possível os estilos pré-definidos do bootstrap, ou os fornecidos no site.ccs;



### Bibliotecas usadas
- Bootstrap v4.6.2 (https://getbootstrap.com)
- Font Awesome Free v5.15.4 (https://fontawesome.com)
- jQuery v3.7.1 (https://jquery.com)
- jQuery Validation Plugin v1.19.5 (https://jqueryvalidation.org)
- Respond.js v1.4.2 (https://github.com/scottjehl/Respond)
