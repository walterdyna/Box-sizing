
Guia Prático: Box Sizing no CSS


O que é o Box Sizing?

O box-sizing é uma propriedade essencial em CSS que determina como o tamanho total de um elemento é calculado, considerando ou não as bordas e o preenchimento.

No exemplo abaixo, todos os elementos na página são configurados para usar o modelo de caixa border-box. Isso significa que o tamanho total do elemento incluirá conteúdo, preenchimento e borda, sem ultrapassar as dimensões especificadas.

* {
    box-sizing: border-box; 
}


Como Funciona na Prática

Considere o seguinte exemplo de um elemento com a classe .box:

.box {
    width: 100px;
    height: 100px;
    background: #ff1493;
    padding: 20px;
    border: 10px solid #0000ff;
}

Neste caso, o box-sizing: border-box; garante que as dimensões totais da .box permaneçam fixas em 100x100 pixels, independentemente do preenchimento e da borda. Sem o border-box, o tamanho total seria a soma do conteúdo, preenchimento e borda, o que poderia resultar em um elemento maior do que o desejado.


Escolhendo entre Content-Box e Border-Box

Content-Box (Padrão): O tamanho do elemento é calculado apenas pelo conteúdo, excluindo preenchimento e borda.

Border-Box: O tamanho total do elemento inclui conteúdo, preenchimento e borda.


Quando Utilizar?

Use border-box quando desejar especificar as dimensões totais do elemento (conteúdo, preenchimento e borda) e garantir que essas dimensões permaneçam constantes.

Use content-box se preferir dimensionar apenas o conteúdo e permitir que preenchimento e borda sejam adicionados ao tamanho total.


Lembre-se de escolher o modelo de caixa que melhor atenda às necessidades específicas de layout do seu projeto. Experimente ambos e determine qual se alinha melhor com suas preferências e requisitos de design.