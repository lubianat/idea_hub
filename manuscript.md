---
author-meta:
- Tiago Lubiana
bibliography:
- content/manual-references.json
date-meta: '2020-11-04'
header-includes: "<!--\nManubot generated metadata rendered from header-includes-template.html.\nSuggest improvements at https://github.com/manubot/manubot/blob/master/manubot/process/header-includes-template.html\n-->\n<meta name=\"dc.format\" content=\"text/html\" />\n<meta name=\"dc.title\" content=\"Project idea\" />\n<meta name=\"citation_title\" content=\"Project idea\" />\n<meta property=\"og:title\" content=\"Project idea\" />\n<meta property=\"twitter:title\" content=\"Project idea\" />\n<meta name=\"dc.date\" content=\"2020-11-04\" />\n<meta name=\"citation_publication_date\" content=\"2020-11-04\" />\n<meta name=\"dc.language\" content=\"en-US\" />\n<meta name=\"citation_language\" content=\"en-US\" />\n<meta name=\"dc.relation.ispartof\" content=\"Manubot\" />\n<meta name=\"dc.publisher\" content=\"Manubot\" />\n<meta name=\"citation_journal_title\" content=\"Manubot\" />\n<meta name=\"citation_technical_report_institution\" content=\"Manubot\" />\n<meta name=\"citation_author\" content=\"Tiago Lubiana\" />\n<meta name=\"citation_author_institution\" content=\"Computational Systems Biology Laboratory, University of S\xE3o Paulo, Brazil\" />\n<meta name=\"citation_author_orcid\" content=\"0000-0003-2473-2313\" />\n<link rel=\"canonical\" href=\"https://lubianat.github.io/idea_hub/\" />\n<meta property=\"og:url\" content=\"https://lubianat.github.io/idea_hub/\" />\n<meta property=\"twitter:url\" content=\"https://lubianat.github.io/idea_hub/\" />\n<meta name=\"citation_fulltext_html_url\" content=\"https://lubianat.github.io/idea_hub/\" />\n<meta name=\"citation_pdf_url\" content=\"https://lubianat.github.io/idea_hub/manuscript.pdf\" />\n<link rel=\"alternate\" type=\"application/pdf\" href=\"https://lubianat.github.io/idea_hub/manuscript.pdf\" />\n<link rel=\"alternate\" type=\"text/html\" href=\"https://lubianat.github.io/idea_hub/v/30c0fa8a3212d2f45798e825f052186eebe50510/\" />\n<meta name=\"manubot_html_url_versioned\" content=\"https://lubianat.github.io/idea_hub/v/30c0fa8a3212d2f45798e825f052186eebe50510/\" />\n<meta name=\"manubot_pdf_url_versioned\" content=\"https://lubianat.github.io/idea_hub/v/30c0fa8a3212d2f45798e825f052186eebe50510/manuscript.pdf\" />\n<meta property=\"og:type\" content=\"article\" />\n<meta property=\"twitter:card\" content=\"summary_large_image\" />\n<link rel=\"icon\" type=\"image/png\" sizes=\"192x192\" href=\"https://manubot.org/favicon-192x192.png\" />\n<link rel=\"mask-icon\" href=\"https://manubot.org/safari-pinned-tab.svg\" color=\"#ad1457\" />\n<meta name=\"theme-color\" content=\"#ad1457\" />\n<!-- end Manubot generated metadata -->"
keywords:
- idea
- project
- idea
lang: en-US
manubot-clear-requests-cache: false
manubot-output-bibliography: output/references.json
manubot-output-citekeys: output/citations.tsv
manubot-requests-cache-path: ci/cache/requests-cache
title: Project idea
...






<small><em>
This manuscript
([permalink](https://lubianat.github.io/idea_hub/v/30c0fa8a3212d2f45798e825f052186eebe50510/))
was automatically generated
from [lubianat/idea_hub@30c0fa8](https://github.com/lubianat/idea_hub/tree/30c0fa8a3212d2f45798e825f052186eebe50510)
on November 4, 2020.
</em></small>

## Authors



+ **Tiago Lubiana**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [0000-0003-2473-2313](https://orcid.org/0000-0003-2473-2313)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [lubianat](https://github.com/lubianat)<br>
  <small>
     Computational Systems Biology Laboratory, University of São Paulo, Brazil
  </small>



## Abstract {.page_break_before}


### Testing Manubot citation
  [@wikidata:Q38114797]



# Reviews

## A review of cell-type annotation tools/methods

- Open collaborative review.

- Questions: what has been proposed so far? Which packages/modules are available?


## A review of single-cell analysis frameworks

- Question: What are the _de facto_ standards for each step? 

- Python / R / Julia / Other

- Seurat / Bioconductor SingleCellExperiment?

- Search on EuropePMC "single-cell RNA sequencing" AND (FIRST_PDATE:2019) AND (((SRC:MED OR SRC:PMC OR SRC:AGR OR SRC:CBA) NOT (PUB_TYPE:"Review")))

- Review top 100. 

Class:

    - Method
    - Primary analysis
    - Reanalysis

Use the [Systematic Review Facility](https://app.syrf.org.uk/home).





# Considerations based on information theory and human communication

(Written in Portuguese)

Modelagem de frases ambíguas

Pa = probabilidades da percepção do ouvinte na perspectiva do falante
Pb = probabilidades a percepção do ouvinte de fato


### Duas opções no modelo: comentário positivo e comentário negativo

P(X_intent = positive_comment) + P(X_intent = negative_comment) = 1

### 3 elementos: a intenção, a fala e a conclusão do ouvinte

X_intent = intenção do falante 
X_spoken = as palavras usadas ("a fala")
Y_guess_about_X_intent  = a conclusão do ouvinte sobre a intenção do falante 

Y_guess_about_X_intent | X_spoken  = a conclusão do ouvinte sobre a intenção do falante  dada a fala

### A resolução de intenção por Bayes

O ouvinte conclui baseado em preconcepções a partir da fala. Por Bayes (exemplificando): 


P(Y_guess_about_X_intent = "positive_comment" | X_spoken = "example") = 

P(X_spoken = "example") * P( X_spoken = "example" | Y_guess_about_X_intent = "positive_comment")


### Exemplificando X_spoken para esclarecer

P(X_spoken = "example") = Probabilidade de você falar "example" exatamente daquele jeito, com aquela escolha de palavras. 
Dada todas as possibilidades de fala, qual é a probabilidade de você falar exatamente aquilo? 

Bem, isso é, rigorosamente, não-modelável, mas podemos estimar com modelos linguísticos probabilísticos. 

Para os fins aqui, vamos supor que há apenas 4 frases possíveis, todas igualmente prováveis _a priori_. 

P(X_spoken == 1) = 0.25
P(X_spoken == 2) = 0.25 
P(X_spoken == 3) = 0.25 
P(X_spoken == 4) = 0.25 


### Exemplificanfo P( X_spoken = "example" | X_intent = "positive_comment")

P(X_spoken = "example" | X_intent = "positive_comment") é a probabilidade de você falar "example" quando sua intenção é positiva. 

Para as 10 frases possíveis, digamos que metade sejam consideradas por você mais positivas e metade mais negativas. Mas você nem sempre
usa a mesma frase quando que passar uma mensagem positiva. Vamos supor que:

Dado a intenção positiva, , por exemplo:

P(X_spoken == 1 | X_intent = "positive_comment") = 0.5 
P(X_spoken == 2 | X_intent = "positive_comment") = 0.3 
P(X_spoken == 3 | X_intent = "positive_comment") = 0.2 
P(X_spoken == 4 | X_intent = "positive_comment") = 0.0 


Dada uma intenção negativa, , por exemplo:

P(X_spoken == 1 | X_intent = "negative_comment") = 0.0 
P(X_spoken == 2 | X_intent = "negative_comment") = 0.2 
P(X_spoken == 3 | X_intent = "negative_comment") = 0.3 
P(X_spoken == 4 | X_intent = "negative_comment") = 0.5 


### Exemplificando Y_guess_about_X_intent para esclarecer

Agora, o ouvinte não sabe o que X_intent é, de fato. O que ele tem é Y_guess_about_X_intent, que é modificada pela fala.
Há uma preconcepção, e essa preconcepção é atualizada. E é isso que o falante tem que pensar: no que a frase significa para 
o ouvinte, e não o que significa para ele. 


Esse chute tem um valor a priori e um a posteriori (Y_guess_about_X_intent|X_spoken).


### Exemplificanfo P( X_spoken = "example" | Y_guess_about_X_intent = "positive_comment")
O ouvinte, então, tem seus modelos mentais de uso de linguagem.

#### Um cenário
Se o ouvinte tem a mesma percepção de uso de vocabulário do falante, então as probabilidadese de repetem:

P(X_spoken == 1 | Y_guess_about_X_intent = "positive_comment") = 0.5 
P(X_spoken == 2 | Y_guess_about_X_intent = "positive_comment") = 0.3 
P(X_spoken == 3 | Y_guess_about_X_intent = "positive_comment") = 0.2 
P(X_spoken == 4 | Y_guess_about_X_intent = "positive_comment") = 0.0 

P(X_spoken == 1 | Y_guess_about_X_intent = "negative_comment") = 0.0 
P(X_spoken == 2 | Y_guess_about_X_intent = "negative_comment") = 0.2 
P(X_spoken == 3 | Y_guess_about_X_intent = "negative_comment") = 0.3 
P(X_spoken == 4 | Y_guess_about_X_intent = "negative_comment") = 0.5 

#### Outro cenário

Mas é possível que, por exemplo, na cultura do ouvinte, a frase 1 tenha uma palavra muito preconceituosa. 
O falante não sabe disso, mas isso pode afeta o ouvinte:

P(X_spoken == 1 | Y_guess_about_X_intent = "positive_comment") = 0.0 
P(X_spoken == 2 | Y_guess_about_X_intent = "positive_comment") = 0.6 
P(X_spoken == 3 | Y_guess_about_X_intent = "positive_comment") = 0.4 
P(X_spoken == 4 | Y_guess_about_X_intent = "positive_comment") = 0.0

P(X_spoken == 1 | Y_guess_about_X_intent = "negative_comment") = 0.4 
P(X_spoken == 2 | Y_guess_about_X_intent = "negative_comment") = 0.1 
P(X_spoken == 3 | Y_guess_about_X_intent = "negative_comment") = 0.2 
P(X_spoken == 4 | Y_guess_about_X_intent = "negative_comment") = 0.3


## O funcionamento e os ruidos do diálogo

Além das probabilidades de fato, a percepção de probabilidades pelo falante tem um papel importante. 

A tarefa objetiva do falante é maximizar a P(Y_guess_about_X_intent = X_intent).

O falante sabe que a informação que o ouvinte tem é o a fala ("X_spoken").


Logo,, na concepção do falante (Pfala) a probabilidade do outro entender aquilo que ele está falando: 
P_fala(Y_guess_about_X_intent|X_spoken) = P_fala(X_spoken) x P_fala(X_spoken|Y_guess_about_X_intent) / P_fala(Y_guess_about_X_intent)

Os diferentes P_fala podem divergir dos P_real, e isso causa conflito de diálogo. 

# Implicações dos fatores latentes

## Divergência sobre percepção de intenção do falante afeta o diálogo
Se Pfala(Y_guess_about_X_intent) e Preal(Y_guess_about_X_intent) são muito diferentes, a comunicação fica complicada.

## Divergência sobre a predisposição do ouvinte entender que alguém com intenção "Y" falaria algo da forma "X"
P_fala(X_spoken/Y_guess_about_X_intent) e Preal(X_spoken/Y_guess_about_X_intent) podem ser diferentes.
Uma pessoa 'grossa' pode usar um conjunto de palavras e achar que está sendo positivo, mas para o interlocutor pode ser negativo. 

## Divergência sobre o uso geral de frases

O último fator que entra no cálculo é o  P(X_spoken). O P_real(X_spoken) é a distribuição de frases para o ouvinte. Se o vocabulário 
é o mesmo, é provável que isso seja parecido para os dois. 

O uso de gírias, por exemplo, pode complicar nesse caso. Se a outra pessoa não conhece uma gíria, a probabilidade de uso dessa frase no
geral é muitoo baixa. 

Para fins práticos, contudo, considerarei Pfala(X_spoken) = Preal(X_spoken), mudando apenas as probabilidades condicionais. 



# TypemakeR

Given a Seurat object, a binarized dataframe and a maximum number of genes per type, 

find the best combination of markers (using AND, OR, NOR, XOR) that better captures the clusters


# TechnotypeR 

A simple annotation package for single-cell RNA-seq data based on the technotype framework.

Reference cell types based on markers.

_sensu stricto_ cell types

 - ID: QXXX

 - Markers:

    - Expresses X OR Y
        - A1
        - A2
    - Expresses X AND Y
        -B
        -C
    - NOT (Expresses X OR Y)
        -D1
        -D2

    - NOT (Expresses X AND Y)
        -F
        -G

Example

ID: Q001
label: "human B cell"

(at least 1)
    - Expresses X OR Y
        - MS4A1
        - CD79A
        - CD79B
(all)
    - Expresses X AND Y

(not express at least 1)
    - NOT (Expresses X OR Y)

(not express all)    
    - NOT (Expresses X AND Y)
        - CD3E
        - CD4
        - CD8A
        - NKG7


Steps:

    - User decides what counts as expressed --> binarization algorithm
    - Apply mask to dataset
    - Cells are labeled with multiple labels.
        - For each mask, test all cells. 
            - If a mask fits, label as technotype (e.g, using dataset_ID_Q001)
            - Relate technotype as a subclass of the uper class (e.g Q001)

## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
