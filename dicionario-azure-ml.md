# Dicionário Básico de Termos - Azure Machine Learning

## Geral e Conceitos Fundamentais

| **Termo**               | **Significado**                                                                 | **Quando, Onde e Porquê Usar**                                                                 | **Comentários**                                                                 |
|--------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------|
| **Ambiente**            | Configuração que define dependências e pacotes necessários para executar um experimento ou pipeline. | Usado para garantir que o código seja executado em um ambiente controlado e reproduzível.     | Pode ser configurado com Conda ou Docker.                                       |
| **CLI**                 | Interface de Linha de Comando para interagir com serviços do Azure.              | Usado para automatizar tarefas e gerenciar recursos do Azure.                                | Requer familiaridade com comandos básicos.                                      |
| **SDK**                 | Kit de Desenvolvimento de Software para interagir com serviços do Azure.        | Usado para desenvolver aplicações que utilizam recursos do Azure Machine Learning.           | Compatível com Python e outras linguagens.                                      |
| **API**                 | Interface de Programação de Aplicações para comunicação entre sistemas.          | Usado para acessar funcionalidades e dados de serviços como Azure ML, de forma programática. | Essencial em integrações e automação de processos.                              |
| **Cluster**             | Conjunto de máquinas virtuais configuradas para treinamento ou inferência de modelos. | Usado para escalar operações de aprendizado de máquina.                                       | Essencial para projetos de larga escala.                                        |
| **Machine Learning**    | Técnica que permite a criação de sistemas que aprendem e melhoram com os dados. | Usado para resolver problemas como previsão, classificação e clustering.                    | Base de todo o processo de Azure ML.                                            |
| **Modelo**              | Representação matemática treinada que faz previsões ou análises.                | Usado para aplicar aprendizado de máquina em dados novos.                                    | Geralmente precisa ser treinado e ajustado.                                     |
| **Pipeline**            | Sequência de etapas automatizadas para treinamento e implantação de modelos.     | Usado para organizar e reproduzir fluxos de trabalho de aprendizado de máquina.              | Facilita a colaboração e automação de processos.                                |
| **AutoML**              | Ferramenta para treinar automaticamente modelos de aprendizado de máquina.      | Usado para acelerar o desenvolvimento sem necessidade de conhecimento avançado.              | Ideal para protótipos rápidos.                                                  |

---

## Dados e Armazenamento

| **Termo**               | **Significado**                                                                 | **Quando, Onde e Porquê Usar**                                                                 | **Comentários**                                                                 |
|--------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------|
| **Blob**                | Tipo de armazenamento no Azure para grandes volumes de dados não estruturados.   | Usado para armazenar imagens, vídeos e outros arquivos grandes.                              | Parte do Azure Storage.                                                         |
| **Datalake**            | Solução de armazenamento para grandes volumes de dados estruturados e não estruturados. | Usado para armazenar e processar dados em escala.                                             | Ideal para análises avançadas e aprendizado de máquina.                         |
| **Ativo de Dados**      | Recurso que contém dados registrados no Azure ML, como arquivos ou tabelas.      | Usado para gerenciar e reutilizar dados em diferentes experimentos e pipelines.              | Facilita a rastreabilidade e a governança de dados.                             |
| **URI**                 | Identificador de recurso uniforme para localizar arquivos ou pastas.            | Usado para acessar dados armazenados localmente ou na nuvem.                                 | Pode ser usado em pipelines e experimentos.                                     |
| **ML Table**            | Abstração para dados tabulares no Azure Machine Learning.                        | Usado para manipular dados estruturados em pipelines e experimentos.                         | Compatível com AutoML e pipelines avançados.                                    |
| **Arquivo URI**         | Identificador de um arquivo armazenado localmente ou na nuvem.                   | Usado para acessar arquivos específicos em pipelines ou experimentos.                        | Útil para manipulação de dados em pipelines.                                    |
| **Pasta URI**           | Identificador que aponta para uma pasta de dados.                               | Usado para organizar e acessar múltiplos arquivos.                                           | Facilita a gestão de dados em projetos.                                         |
| **JSON**                | Formato leve de dados para transmissão de informações.                          | Usado para comunicação entre APIs e armazenamento de metadados.                             | Amplamente utilizado em sistemas modernos.                                      |
| **Data Drift**          | Mudanças nos dados que podem impactar a performance do modelo.                  | Usado para monitorar e ajustar modelos em produção.                                          | Importante para garantir precisão contínua.                                     |

---

## Processos e Automação

| **Termo**               | **Significado**                                                                 | **Quando, Onde e Porquê Usar**                                                                 | **Comentários**                                                                 |
|--------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------|
| **Experimentos**        | Unidade de execução de um processo de aprendizado de máquina.                    | Usado para testar e validar modelos de aprendizado de máquina.                               | Permite rastrear resultados e reproduzir experimentos.                          |
| **Agendamento**         | Processo de automatizar a execução de pipelines em horários definidos.          | Usado para criar fluxos de trabalho repetitivos.                                              | Importante para treinamentos recorrentes.                                       |
| **Automação**           | Uso de ferramentas para executar tarefas sem intervenção manual.                | Usado para aumentar a eficiência e consistência de processos.                               | Amplamente utilizado em aprendizado de máquina e operações de TI.               |
| **ML Lifecycle**        | Ciclo de vida do aprendizado de máquina, que inclui desenvolvimento, treinamento, implantação e monitoramento. | Usado para gerenciar projetos de ML.                                                         | Essencial para governança e rastreabilidade.                                    |
| **Validação Cruzada**   | Técnica para avaliar a performance do modelo dividindo os dados em múltiplas partes. | Usado para garantir que o modelo generaliza bem para novos dados.                            | Minimiza risco de overfitting.                                                  |

---

## Desenvolvimento e Ferramentas

| **Termo**               | **Significado**                                                                 | **Quando, Onde e Porquê Usar**                                                                 | **Comentários**                                                                 |
|--------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------|
| **Notebook**            | Interface interativa para desenvolvimento e execução de código.                  | Usado para explorar dados e desenvolver modelos de aprendizado de máquina.                   | Compatível com Jupyter e Azure Machine Learning Studio.                         |
| **Conda**               | Gerenciador de pacotes e ambientes para Python.                                  | Usado para criar ambientes isolados com dependências específicas.                            | Compatível com o Azure Machine Learning.                                        |
| **Docker**              | Plataforma para criar, executar e gerenciar contêineres.                        | Usado para criar ambientes isolados e portáveis para execução de modelos.                    | Facilita a replicação de ambientes.                                             |
| **Docker File**         | Arquivo que define como um contêiner Docker será construído.                     | Usado para criar imagens Docker personalizadas.                                               | Necessário para configurar ambientes específicos.                               |
| **YAML**                | Formato de arquivo para configuração de ambientes e pipelines.                   | Usado para definir parâmetros e dependências em projetos de aprendizado de máquina.          | Simples e legível, mas requer atenção à indentação.                             |
| **Interface Web**       | Ferramenta visual para gerenciar recursos do Azure Machine Learning.            | Usada para gerenciar pipelines e modelos sem precisar de linha de comando.                  | Excelente para iniciantes.                                                      |
| **Linguagem R**         | Linguagem de programação popular para estatísticas e aprendizado de máquina.     | Usado para análises avançadas e modelos estatísticos.                                         | Compatível com o Azure Machine Learning.                                        |

---

## Modelos e Inferências

| **Termo**               | **Significado**                                                                 | **Quando, Onde e Porquê Usar**                                                                 | **Comentários**                                                                 |
|--------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------|
| **Inference Cluster**   | Cluster configurado para executar inferências de modelos implantados.            | Usado para escalar a execução de inferências em produção.                                     | Ideal para aplicações que exigem alta disponibilidade.                          |
| **Treinamento**          | Processo de ajuste de um modelo de aprendizado de máquina com base em dados.    | Usado para criar modelos precisos que generalizem bem em novos dados.                        | Passo fundamental em ML.                                                        |
| **Validação**            | Processo de avaliação da qualidade do modelo usando dados de teste.             | Usado para verificar se o modelo está funcionando corretamente.                              | Essencial para prevenir overfitting.                                            |
| **Regressão**            | Técnica usada para prever valores contínuos.                                    | Usado em problemas como previsão de preços ou demanda.                                       | Base para modelos preditivos.                                                   |
| **Classificação**        | Técnica para prever categorias ou rótulos em dados.                             | Usado em tarefas como detecção de spam ou diagnóstico médico.                                | Essencial para modelos supervisionados.                                         |

---
