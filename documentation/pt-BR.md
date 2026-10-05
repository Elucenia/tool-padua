<!-- ELUCENIA technical documentation · padua · pt-BR · no clinical/professional/rights approval -->

# Escore de Pádua

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/padua)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Câncer ativo (metástase ou quimio/radioterapia nos últimos 6 meses)

`cancer`

### TEV prévio (exceto trombose venosa superficial)

`tev`

### Mobilidade reduzida (repouso no leito, com ida ao banheiro, por ≥ 3 dias)

`mobilidade`

### Trombofilia conhecida

`trombofilia`

### Trauma ou cirurgia no último mês

`trauma`

### Idade ≥ 70 anos

`idade`

### Insuficiência cardíaca e/ou respiratória

`icc`

### IAM agudo ou AVC isquêmico

`iam`

### Infecção aguda e/ou doença reumatológica

`infeccao`

### Obesidade (IMC ≥ 30 kg/m²)

`obesidade`

### Tratamento hormonal em curso

`hormonio`

## Edição do método

Padua Prediction Score/Barbar 2010:11 fatores,0–20; paciente clínicohospitalizado

## Fórmula documentada

3 pontos: câncer ativo, TEV prévio, mobilidade reduzida, trombofilia · 2 pontos: trauma ou cirurgia recente · 1 ponto: idade ≥ 70, insuficiência cardíaca/respiratória, IAM ou AVC isquêmico, infecção aguda ou doença reumatológica, obesidade, terapia hormonal. Máximo: 20.

## Limites e população

O Padua foi estudado em pacientes clínicos internados em medicina interna, com seguimento de tromboembolismo sintomático até 90 dias. A estratificação trombótica deve ser acompanhada de avaliação de sangramento, contraindicações e protocolo de profilaxia. O total não substitui essa análise nem implica aplicação automática à população cirúrgica.

## Referências

- [Barbar S et al. A risk assessment model for the identification of hospitalized medical patients at risk for venous thromboembolism: the Padua Prediction Score. J Thromb Haemost, 2010.](https://doi.org/10.1111/j.1538-7836.2010.04044.x)

- [Kahn SR et al. Prevention of VTE in nonsurgical patients: antithrombotic therapy and prevention of thrombosis, 9th ed: American College of Chest Physicians evidence-based clinical practice guidelines. Chest, 2012.](https://doi.org/10.1378/chest.11-2296)

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
