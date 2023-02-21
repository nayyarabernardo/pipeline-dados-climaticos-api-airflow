# Pipeline de dados com Airflow e a API Timeline Weather 🌧️

## Coleta e processamento de informações meteorológicas em Python


Este repositório contém um pipeline de dados implementado utilizando o Airflow para coletar informações meteorológicas da API Timeline Weather para a cidade de Boston. O pipeline é executado semanalmente e coleta dados dos últimos sete dias.

**Índice**
## Índice

- [Sobre a API Timeline Weather](#sobre-a-api-timeline-weather)
- [Sobre o pipeline de dados](#sobre-o-pipeline-de-dados)
- [Como executar o pipeline](#como-executar-o-pipeline)
- [Considerações](#considerações)
- [Licença](#licença)
- [Contribuição](#contribuição)
- [Links](#links)


## Sobre a API Timeline Weather

A API Timeline Weather é uma API que fornece informações meteorológicas históricas e em tempo real para locais em todo o mundo. É uma ferramenta valiosa para qualquer pessoa que precise acessar informações meteorológicas precisas e confiáveis.

Todas as solicitações para a API Timeline Weather usam o seguinte formulário:

```bash
https://weather.visualcrossing.com/VisualCrossingWebServices/rest/services/timeline/[location]/[date1]/[date2]?key=YOUR_API_KEY
```

## Sobre o pipeline de dados

Este pipeline foi desenvolvido utilizando o Airflow, uma plataforma de gerenciamento de fluxo de trabalho em código aberto que permite agendar e executar tarefas em momentos específicos. O pipeline foi projetado para coletar dados meteorológicos da API Timeline Weather para a cidade de Boston uma vez por semana.

O pipeline coleta dados dos últimos sete dias para fornecer informações meteorológicas recentes para a cidade. As informações coletadas incluem a temperatura, a pressão atmosférica, a umidade, a velocidade do vento e a direção do vento.

O pipeline foi projetado para garantir a qualidade dos dados coletados. Ele inclui etapas para verificar a integridade dos dados e lidar com quaisquer erros ou exceções que possam ocorrer durante a execução do pipeline.

## Como executar o pipeline

Para executar o pipeline, é necessário ter o Airflow instalado e configurado em sua máquina. Além disso, é necessário criar uma conta na API Timeline Weather e obter uma chave de API válida.

Uma vez que o Airflow esteja configurado e a chave de API esteja disponível, é possível agendar e executar o pipeline por meio da interface do Airflow. O pipeline está configurado para executar automaticamente uma vez por semana, mas também é possível executá-lo manualmente, se necessário.

## Considerações

Este pipeline de dados é um exemplo de como o Airflow pode ser utilizado para coletar e processar informações de fontes externas, como a API Timeline Weather. O pipeline foi projetado para ser fácil de usar e configurar, permitindo que qualquer pessoa possa executá-lo e coletar informações meteorológicas precisas e atualizadas para a cidade de Boston.

## Licença

Este projeto está disponível sob a licença [APACHE](https://www.apache.org/licenses/LICENSE-2.0).

## Contribuição

Este projeto é aberto a contribuições. Se você deseja melhorar ou adicionar recursos, sinta-se à vontade para criar uma solicitação pull ou entrar em [contato](https://www.linkedin.com/in/nayyarabernardo).

## Links

- [Documentation Apache Airflow](https://airflow.apache.org/docs/stable/)
- [Documentation Timeline Weather API ](https://www.visualcrossing.com/resources/documentation/weather-api/timeline-weather-api/)
