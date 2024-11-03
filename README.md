# Sistema de Monitoramento de Temperatura e Umidade

Este projeto tem como objetivo automatizar a captação da temperatura e umidade do ar ao longo do dia, permitindo a criação de um histórico dessas variáveis climáticas. Através da coleta contínua de dados, o sistema facilita a visualização e análise das variações climáticas, possibilitando a geração de gráficos que representam essas informações de maneira mais precisa.

## Tecnologias Utilizadas

- **Python**: A linguagem de programação principal utilizada para desenvolver a aplicação.
- **Tkinter**: Biblioteca utilizada para criar uma interface gráfica amigável, permitindo que o usuário interaja facilmente com a aplicação.
- **BeautifulSoup**: Biblioteca para realizar a raspagem de dados (web scraping) de sites de previsão do tempo, extraindo informações relevantes sobre temperatura e umidade.
- **datetime**: Módulo que permite capturar e formatar a data e hora atuais, assegurando que cada registro de temperatura e umidade seja acompanhado por um timestamp.
- **openpyxl**: Biblioteca utilizada para manipulação de arquivos Excel, permitindo armazenar os dados coletados em uma planilha organizada, onde cada entrada inclui a data, hora, temperatura e umidade.
- **Selenium**: Ferramenta utilizada para automatizar a interação com sites que podem exigir navegação dinâmica ou que utilizam JavaScript para carregar os dados.

## Funcionamento do Sistema

1. **Interface Gráfica**: O usuário inicia a aplicação através de uma interface desenvolvida em Tkinter, onde pode iniciar e parar a coleta de dados.
2. **Coleta de Dados**: Ao iniciar a coleta, o sistema utiliza o Selenium para acessar um site de previsão do tempo. O BeautifulSoup é utilizado para extrair os dados de temperatura e umidade disponíveis.
3. **Registro dos Dados**: Cada vez que os dados são capturados, a data e a hora atuais são registradas utilizando o módulo datetime. As informações coletadas são então armazenadas em uma planilha Excel, com cada linha contendo a data, hora, temperatura e umidade.
4. **Visualização**: O histórico de dados coletados pode ser utilizado para gerar gráficos em ferramentas externas (como Excel ou bibliotecas de visualização de dados em Python), permitindo uma análise visual das variações ao longo do dia.

## Benefícios do Sistema

- **Automatização**: Elimina a necessidade de anotações manuais, reduzindo o erro humano e economizando tempo.
- **Histórico de Dados**: Permite o armazenamento sistemático de dados, facilitando análises futuras.
- **Visualização de Dados**: Gera insights sobre as variações de temperatura e umidade ao longo do dia, ajudando em previsões e estudos climáticos.

Este sistema proporciona uma solução eficiente e prática para a monitorização do clima, tornando a coleta de dados mais acessível e organizada.
