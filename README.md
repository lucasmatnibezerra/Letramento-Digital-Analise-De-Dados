# Letramento Digital em Inteligência Artificial (UFPA / Fundação Guamá)

Repositório de apoio ao curso gratuito de **Letramento Digital em Inteligência Artificial** promovido pela Fundação Guamá. Este espaço reúne dados, notebooks e orientações para atividades práticas de análise exploratória e compreensão inicial de conceitos ligados a dados e IA, com foco em aplicações contextualizadas à realidade amazônica e à inclusão digital.

## Contexto do Curso
- **Carga horária:** 120 horas (04 de agosto a 19 de dezembro)
- **Formato:** Aulas presenciais (turno da manhã) no Parque de Ciência e Tecnologia Guamá
- **Vagas:** 20 (destinadas a moradores dos bairros Guamá e Terra Firme, estudantes de universidades do entorno e estudantes de escolas públicas próximas)
- **Público-alvo:** Pessoas a partir de 16 anos com conhecimentos básicos de informática
- **Foco formativo:** Inclusão digital, fundamentos de programação em Python, engenharia de prompt, noções introdutórias de machine learning, visão computacional e ética no uso de IA.
- **Contato:** letramento.digital@fundacaoguama.org.br

## Objetivos do Repositório
Este repositório serve para:
1. Apoiar as aulas de análise de dados e reflexão sobre qualidade e interpretação de variáveis.
2. Disponibilizar datasets e notebooks estruturados para exploração guiada pelos(as) alunos(as).
3. Registrar resultados de exercícios e produções das turmas.
4. Incentivar boas práticas básicas de organização e documentação desde o início do aprendizado.

## Estrutura dos Arquivos
| Arquivo | Descrição |
|---------|-----------|
| `StressLevelDataset.csv` | Conjunto de dados utilizado para atividades de análise exploratória. Contém variáveis relacionadas a fatores psicossociais e um índice de estresse (`stress_level`). |
| `kidsfeet.dat.txt` | Arquivo de dados auxiliar (exemplo pedagógico para operações de leitura e manipulação simples). Pode ser usado em exercícios adicionais. |
| `Análise_de_dados.ipynb` | Notebook de referência (aulas). Contém células demonstrativas, anotações e exemplos de exploração inicial dos dados. Pode incluir gráficos, estatísticas e explicações teóricas. |
| `Template_Analise.ipynb` | Modelo (template) limpo para os(as) alunos(as) preencherem durante a análise exploratória. Cada célula traz apenas orientações conceituais (sem código pronto). |
| `README.md` | Este documento de descrição e orientação geral. |

## Sobre o Dataset Principal (`StressLevelDataset.csv`)
Cada linha representa um(a) participante/análise individual. As colunas incluem variáveis numéricas discretas que representam níveis, índices ou presença/ausência de características (em alguns casos codificadas de forma ordinal ou binária). A variável alvo para discussão exploratória é `stress_level`.

### Dicionário de Variáveis (Resumo Interpretativo)
Observação: Os significados abaixo são inferências pedagógicas para fins de letramento; podem ser ajustados conforme documentação formal (se fornecida futuramente).
| Coluna | Interpretação Sugerida | Tipo (proposto) | Observação |
|--------|------------------------|-----------------|------------|
| `anxiety_level` | Nível relativo de ansiedade | Numérica discreta | Escala ordinal (valores inteiros) |
| `self_esteem` | Indicador de autoestima | Numérica discreta | Escala positiva; valores altos indicam maior autoestima |
| `mental_health_history` | Histórico de saúde mental (0/1) | Categórica binária | 1 pode indicar histórico positivo de diagnóstico/atendimento |
| `depression` | Indicador de sintomas depressivos | Numérica discreta | Pode correlacionar-se com ansiedade e estresse |
| `headache` | Frequência/nível de queixas de dor de cabeça | Numérica discreta | Potencial fator físico associado |
| `blood_pressure` | Indicador relativo de pressão arterial | Numérica discreta | Interpretar com cautela (sem unidades clínicas) |
| `sleep_quality` | Qualidade do sono | Numérica discreta | Valores diferentes podem sinalizar impacto em `stress_level` |
| `breathing_problem` | Indício de dificuldade respiratória | Numérica discreta / Categórica | Possível fator fisiológico |
| `noise_level` | Exposição percebida a ruído | Numérica discreta | Pode relacionar-se a ambiente de estudo |
| `living_conditions` | Condição percebida de moradia | Numérica discreta | Interpretação socioambiental |
| `safety` | Percepção de segurança | Numérica discreta | Pode moderar níveis de estresse |
| `basic_needs` | Atende necessidades básicas | Numérica discreta | Níveis menores podem associar-se a maior estresse |
| `academic_performance` | Desempenho acadêmico percebido | Numérica discreta | Variável de interesse em cruzamentos |
| `study_load` | Carga de estudo | Numérica discreta | Possível fator de pressão |
| `teacher_student_relationship` | Relação com docentes | Numérica discreta | Clima acadêmico |
| `future_career_concerns` | Preocupações com carreira futura | Numérica discreta | Potencial preditor de estresse |
| `social_support` | Apoio social percebido | Numérica discreta | Pode atuar como fator protetor |
| `peer_pressure` | Pressão de pares | Numérica discreta | Possível fator de risco |
| `extracurricular_activities` | Participação em atividades extracurriculares | Numérica discreta | Pode atuar como equilíbrio ou sobrecarga |
| `bullying` | Experiências de bullying | Numérica discreta / Categórica | Atenção ética na interpretação |
| `stress_level` | Nível geral de estresse percebido | Numérica discreta (Alvo) | Variável central de análise exploratória |

## Fluxo Sugerido para Estudo (Uso do Template)
1. Abrir o `Template_Analise.ipynb` e preencher seção a seção.
2. Mapear tipos de variáveis e escalas.
3. Investigar distribuições individuais (variáveis mais concentradas, assimetrias, valores extremos).
4. Relacionar variáveis de suporte/risco com `stress_level` de forma descritiva.
5. Produzir um resumo interpretativo (não apenas estatístico).
6. Registrar limitações: tamanho da amostra, ausência de metadados oficiais, escalas arbitrárias.

## Boas Práticas Recomendadas
- Trabalhe com cópia do dataset se fizer transformações exploratórias.
- Documente decisões em texto: por que ignorou ou destacou uma variável?
- Evite interpretar causalidade (apenas associação/descrição inicial).
- Mantenha consistência de nomenclatura e idioma nas anotações.

## Como Contribuir (Quando Aberto a Contribuições)
1. Criar branch a partir de `main`.
2. Adicionar notebooks ou melhorias documentais seguindo padrão existente.
3. Incluir descrição clara no início de novos notebooks.
4. Submeter Pull Request descrevendo objetivo pedagógico da alteração.

## Contato
Dúvidas ou sugestões: letramento.digital@fundacaoguama.org.br

---
Material em construção. Este repositório evoluirá conforme as turmas avancem e novas necessidades pedagógicas forem identificadas.
