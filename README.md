# Trabalho Prático 1 - Inteligência Artificial

## Informações do Projeto

**Disciplina:** Inteligência Artificial (IIA)  
**Ano Letivo:** 2024/2025  
**Trabalho:** TP1 - Simulação de Aspiradores Autônomos

## Autores

- **Duarte Santos** - 2022149622
- **Gustavo Costa** - 2023145800

## Descrição

Este projeto implementa uma simulação de aspiradores autônomos utilizando NetLogo. Os aspiradores são agentes inteligentes capazes de:

- Navegar pelo ambiente
- Aspirar lixo (patches vermelhos)
- Recarregar energia em estações de carregamento (patches azuis)
- Despejar lixo coletado em depósitos (patches verdes)
- Evitar obstáculos (patches brancos)
- Lidar com tapetes que reduzem a velocidade (patches cinzentos)
- Reproduzir-se (opcional)
- Lidar com defeitos e falhas (opcional)

## Estrutura do Projeto

```
Trabalho_pratico/
├── tp1.nlogo                          # Código fonte da simulação NetLogo
├── IIA_2425_TP1.pdf                   # Enunciado do trabalho prático
├── DuarteSantos_2022149622_GustavoCosta_2023145800.pdf  # Relatório do trabalho
└── README.md                          # Este ficheiro
```

## Requisitos

- **NetLogo 6.4.0** ou superior

## Como Usar

1. Abra o NetLogo
2. Carregue o ficheiro `tp1.nlogo`
3. Configure os parâmetros na interface:
   - **nCarregadores**: Número de estações de carregamento
   - **pLixo**: Percentagem de lixo no ambiente
   - **nAspiradores**: Número inicial de aspiradores
   - **nEnergia**: Energia inicial dos aspiradores
   - **nCapacidade**: Capacidade máxima de lixo
   - **nIrCarregar**: Nível de energia para ir carregar
   - **tDespejar**: Tempo necessário para despejar
   - **tCarga**: Tempo necessário para carregar
   - **reproducao?**: Ativar/desativar reprodução
   - **tapete?**: Ativar/desativar tapetes
   - **defeitos-aspirador?**: Ativar/desativar defeitos nos aspiradores

4. Clique em **SETUP** para inicializar a simulação
5. Clique em **GO** para iniciar a simulação

## Funcionalidades Implementadas

### Comportamento dos Aspiradores

- **Navegação**: Movimento inteligente pelo ambiente
- **Aspiração**: Coleta de lixo quando encontrado
- **Gestão de Energia**: Recarregamento automático quando a energia está baixa
- **Gestão de Capacidade**: Despejo automático quando a capacidade está cheia
- **Evitação de Obstáculos**: Detecção e contorno de paredes e obstáculos
- **Memória de Localizações**: Lembrança da localização de carregadores e depósitos
- **Comunicação**: Partilha de informação entre aspiradores próximos
- **Reprodução**: Capacidade de criar novos aspiradores (opcional)
- **Defeitos**: Simulação de falhas e avarias (opcional)

### Elementos do Ambiente

- **Lixo (Vermelho)**: Objetivo principal - deve ser aspirado
- **Carregadores (Azul)**: Estações de recarga de energia
- **Depósitos (Verde)**: Locais para despejar lixo coletado
- **Obstáculos (Branco)**: Paredes que bloqueiam o movimento
- **Tapetes (Cinzento)**: Reduzem a velocidade de movimento
- **Espaço Livre (Preto)**: Área navegável

## Parâmetros da Simulação

| Parâmetro | Descrição | Valor Padrão |
|-----------|-----------|--------------|
| nCarregadores | Número de estações de carregamento | 5 |
| pLixo | Percentagem de lixo no ambiente | 40 |
| nAspiradores | Número inicial de aspiradores | 10 |
| nEnergia | Energia inicial dos aspiradores | 100 |
| nCapacidade | Capacidade máxima de lixo | 15 |
| nIrCarregar | Nível de energia para ir carregar | 65 |
| tDespejar | Tempo necessário para despejar | 20 |
| tCarga | Tempo necessário para carregar | 20 |

## Experimentos

O modelo inclui dois experimentos predefinidos:

1. **experiment**: Experimento base com configurações padrão
2. **experimento_vAgentes**: Experimento com múltiplos agentes e tapetes ativados

## Observações

- Os aspiradores morrem quando a energia chega a zero
- Os aspiradores com defeitos têm um número limitado de movimentos antes de falhar
- A reprodução só ocorre quando a energia está no máximo
- Os tapetes reduzem a velocidade de movimento para 0.25 unidades por tick

## Licença

Este projeto foi desenvolvido para fins académicos no âmbito da disciplina de Inteligência Artificial.

## Contacto

Para questões sobre este projeto, contacte os autores através dos números de estudante indicados acima.

