# IA-751 - Instrumentação Biomédica Avançada

## Código de Simulação Computacional De Reconstrução TomográficaPor Retroprojeção Filtrada

O código de análise foi feito na extensão para uso do [Live Editor](https://www.mathworks.com/videos/using-the-live-editor-117940.html) do MATLAB. Ao abrir o software, na aba Live Editor, basta clicar no botão verde de `Run` ou `Run all` no código `main.mlx`.

Texto relativo a tarefa de análise das imagens tomográficas pode ser consultado [neste repositório](https://github.com/larissahmendes/ct-reconstruction/blob/main/monografia.pdf).

Este repositório contem os seguintes arquivos:

  **1.**  Imagens exemplo para reconstrução

É necessário rodar o código para cada imagem separadamente. Basta deixar descomentado a opção desejada habilitando uma definição de `imageData`.

```
% Sheep-Logan phantom

imageData=phantom('Modified Shepp-Logan',512); % 512 specifies the number of rows and columns in the phantom image.

% Padrao SMTE

%imageData=double(imread('smpte.jpg'));

% Specimen from the Visible Human Male - Head subset

%imageData=double(imread('m_vm1125.t1.png'));
```

  **2.**  Códigos de análise
  
    * main.mlx: código principal de reconstrução
    * retroprojecaoFiltrada2D.mlx: função para aplicação de filtro para a retroprojeço filtrada
    * myButter.mlx: código para aplicação de filtro Butterworth

### Referências

[1] Mark   Bangert.Ct   reconstruction   package.https://www.mathworks.com/matlabcentral/fileexchange/34608-ct-reconstruction-package,MA-TLAB Central File Exchange. Retrieved November 24, 2020.

[2]  Ricardo Grossi Dantas. Simulação computacional de reconstrução tomográfica por retroprojeçãofiltrada.



 
