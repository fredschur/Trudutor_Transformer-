# Modelo Transformer para Tradução de Português para Inglês

Este notebook implementa um modelo Transformer para traduzir sentenças do português para o inglês. Ele segue uma versão simplificada da arquitetura Transformer introduzida no artigo ["Attention is All You Need"](https://arxiv.org/abs/1706.03762) por Vaswani et al.

## Visão Geral

- **Carregamento e Pré-processamento de Dados**: Utiliza o conjunto de dados `ted_hrlr_translate/pt_to_en` do TensorFlow Datasets. O conjunto de dados é pré-processado usando tokenização subword para lidar eficazmente com palavras desconhecidas.

- **Arquitetura do Modelo**: Constrói um modelo Transformer com hiperparâmetros personalizáveis, incluindo o número de camadas, dimensões do modelo e número de cabeças de atenção. O modelo incorpora codificação posicional, mecanismos de atenção multi-cabeças e redes neurais feed-forward.

- **Loop de Treinamento**: Implementa um loop de treinamento com cálculo de perda e atualizações de gradientes usando o otimizador Adam. O modelo é treinado ao longo de várias épocas com checkpoints para monitorar o progresso.

## Positivos

- **Implementação Simplificada**: Ao simplificar o código e focar nos componentes essenciais, torna-se mais acessível para aqueles que são novos em Transformers ou em deep learning em geral.

- **Aplicação Prática**: Demonstra uma aplicação real de tradução automática, destacando a utilidade prática dos modelos Transformer.

## Negativos

- **Tempo de Treinamento**: Devido a limitações de recursos, o modelo pode não ter sido treinado por tempo suficiente para alcançar traduções de alta qualidade, potencialmente afetando seu desempenho.

- **Simplificações**: Algumas funcionalidades avançadas e otimizações presentes no artigo original do Transformer foram omitidas, o que pode limitar a eficácia do modelo em tarefas de tradução mais complexas.

- **Avaliação Limitada**: O notebook foca principalmente na perda e em acurácia básica, faltando métricas de avaliação mais sofisticadas.
