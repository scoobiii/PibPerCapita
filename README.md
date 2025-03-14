  # PibPerCapita Nacional | Marica RJ | Noruega
  
    2003. US$3000 | US$2000.
    2013. US$13.400,00.
    2014. .
    2015. .
    2016. .
    2017. .
    2018. .
    2019. .  US$8000 | US$100.000,00
    2020. .
    2021. .
    2022. .
    2023. .
    2024. .


Aqui está a organização dos dados fornecidos em um formato JSON estruturado, seguido de uma explicação sobre como gerar visualizações de **Treemap** e **Sankey**. Além disso, incluí uma estimativa sobre a proporção do PIB que entra e sai pelo orçamento normal, secreto e emendas parlamentares.

---

### **JSON Estruturado**

```json
{
  "PIB_Brasil": {
    "total": "100%",
    "setores": {
      "servicos": "67%",
      "industrial": "27.5%",
      "agricola": "5.5%"
    },
    "economia_informal_ilegal": {
      "total": "15%",
      "jogos_apostas": {
        "total": "1%",
        "apostas_esportivas": "0.5%",
        "cassinos_ilegais": "0.2%",
        "jogo_do_bicho": "0.3%"
      },
      "comercio_servicos_informais": {
        "total": "5%",
        "vendas_rua": "2%",
        "servicos_sem_nota": "1.5%",
        "produtos_falsificados": "1%",
        "transporte_clandestino": "0.5%"
      },
      "contrabando_descaminho": {
        "total": "3%",
        "cigarros_ilegais": "1%",
        "eletronicos_sem_impostos": "1%",
        "remedios_ilegais": "0.5%",
        "outros_produtos": "0.5%"
      },
      "trafico_drogas_crime_organizado": {
        "total": "5%",
        "trafico_drogas": "2%",
        "roubo_revenda_cargas": "1%",
        "extorsao_milicias": "1%",
        "lavagem_dinheiro": "1%"
      },
      "trabalho_escravo_exploracao_ilegal": {
        "total": "1%",
        "garimpo_ilegal": "0.5%",
        "exploracao_madeira": "0.3%",
        "trabalho_escravo": "0.2%"
      }
    },
    "distribuicao_estados": {
      "sao_paulo": "31.1%",
      "rio_de_janeiro": "11.4%",
      "minas_gerais": "9.0%",
      "rio_grande_do_sul": "6.1%",
      "parana": "5.9%",
      "bahia": "4.6%",
      "santa_catarina": "4.0%",
      "distrito_federal": "3.3%",
      "goias": "3.2%",
      "pernambuco": "2.5%",
      "ceara": "2.4%",
      "para": "2.3%",
      "mato_grosso": "2.1%",
      "maranhao": "1.8%",
      "espirito_santo": "1.7%",
      "amazonas": "1.4%",
      "paraiba": "1.4%",
      "rio_grande_do_norte": "0.9%",
      "mato_grosso_do_sul": "0.9%",
      "alagoas": "0.8%",
      "piaui": "0.7%",
      "sergipe": "0.7%",
      "rondonia": "0.6%",
      "tocantins": "0.6%",
      "acre": "0.2%",
      "amapa": "0.2%",
      "roraima": "0.2%"
    },
    "distribuicao_regioes": {
      "sudeste": "53.3%",
      "sul": "16.6%",
      "nordeste": "13.8%",
      "centro_oeste": "10.6%",
      "norte": "5.7%"
    }
  },
  "orçamento_publico": {
    "carga_tributaria": "33% do PIB",
    "destino": {
      "governo_federal": "20% do PIB",
      "governos_estaduais": "8% do PIB",
      "governos_municipais": "5% do PIB"
    },
    "orçamento_secreto": {
      "estimativa": "1.5% do PIB",
      "descricao": "Recursos alocados sem transparência, como emendas de relator e fundos especiais."
    },
    "emendas_parlamentares": {
      "estimativa": "0.5% do PIB",
      "descricao": "Recursos direcionados por deputados e senadores para projetos específicos."
    }
  }
}
```

---

### **Como Gerar Visualizações**

#### **1. Treemap**
- **Ferramentas**: Use **Flourish**, **RAWGraphs** ou **Tableau**.
- **Dados**: Utilize o JSON acima, especialmente os campos `economia_informal_ilegal` e `distribuicao_estados`.
- **Exemplo**:
  - Nível 1: Setores (Serviços, Industrial, Agrícola).
  - Nível 2: Subsetores (Economia Informal, Jogos e Apostas, etc.).
  - Nível 3: Detalhes (Apostas Esportivas, Cassinos Ilegais, etc.).

#### **2. Sankey**
- **Ferramentas**: Use **Flourish** ou **RAWGraphs**.
- **Dados**: Utilize o JSON acima, especialmente os campos `economia_informal_ilegal` e `distribuicao_regioes`.
- **Exemplo**:
  - Nós: Setores (Serviços, Industrial, Agrícola).
  - Fluxos: Movimentação de recursos entre setores e regiões.

---

### **Orçamento Público e Emendas**

#### **Estimativas**:
1. **Orçamento Normal**:
   - Representa a maior parte do PIB, com **33%** destinados à carga tributária.
   - Distribuição:
     - Governo Federal: **20% do PIB**.
     - Governos Estaduais: **8% do PIB**.
     - Governos Municipais: **5% do PIB**.

2. **Orçamento Secreto**:
   - Estimativa: **1.5% do PIB**.
   - Descrição: Recursos alocados sem transparência, como emendas de relator e fundos especiais.

3. **Emendas Parlamentares**:
   - Estimativa: **0.5% do PIB**.
   - Descrição: Recursos direcionados por deputados e senadores para projetos específicos.

---

### **Visualização Sugerida**
- **Sankey**:
  - Nós: Orçamento Normal, Orçamento Secreto, Emendas Parlamentares.
  - Fluxos: Destino dos recursos (Governo Federal, Estados, Municípios).
- **Treemap**:
  - Nível 1: Orçamento Total.
  - Nível 2: Orçamento Normal, Secreto, Emendas.
  - Nível 3: Detalhes (Governo Federal, Estados, Municípios).

---

