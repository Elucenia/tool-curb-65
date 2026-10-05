<!-- ELUCENIA technical documentation · curb-65 · pt-BR · no clinical/professional/rights approval -->

# CURB-65

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/curb-65)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Confusão mental (desorientação nova no tempo, espaço ou pessoa)

`c`

### Ureia \> 42 mg/dL (\> 7 mmol/L)

`u`

### FR ≥ 30 irpm

`r`

### PA sistólica \< 90 mmHg ou diastólica ≤ 60 mmHg (Blood pressure)

`b`

### Idade ≥ 65 anos

`i`

## Edição do método

CURB 65/Lim 2003:confusão, ureia\>7 mmol/L, FR≥30, PA, idade≥65; 0–5

## Fórmula documentada

Um ponto para cada item: Confusão, Ureia \> 7 mmol/L, Respiração ≥ 30/min, Baixa pressão (PAS \< 90 ou PAD ≤ 60 mmHg) e idade ≥ 65. Máximo: 5.

O CRB-65 é o mesmo escore sem a ureia (0 a 4), para uso sem laboratório.

## Limites e população

O CURB-65 de 2003 foi derivado e validado em adultos hospitalizados com pneumonia adquirida na comunidade, usando dados da avaliação inicial e mortalidade em 30 dias. Idade ≥ 65 é um componente do escore, não a idade mínima de elegibilidade. Os limiares originais usam ureia \> 7mmol/L, FR ≥ 30/min e PAS \< 90 ou PAD ≤ 60 mmHg. Exclusões e uso em outras populações exigem leitura do protocolo completo.

## Referências

- [Lim WS et al. Defining community acquired pneumonia severity on presentation to hospital: an international derivation and validation study. Thorax, 2003.](https://doi.org/10.1136/thorax.58.5.377)

- [Lim WS et al. BTS guidelines for the management of community acquired pneumonia in adults: update 2009. Thorax, 2009.](https://doi.org/10.1136/thx.2009.121434)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
