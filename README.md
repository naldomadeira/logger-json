# logger-json

Uma biblioteca leve para geração de logs em formato JSON, facilitando a integração com sistemas de monitoramento e análise de logs. Perfeita para aplicações Node.js que necessitam de um sistema de log estruturado e facilmente pesquisável.

## Características

- **Simples e Fácil de Usar**: Interface minimalista para geração de logs.
- **Flexível**: Suporta diferentes níveis de log (info, debug, warn, error).
- **Integração Fácil**: Projetada para integrar-se facilmente com a maioria dos sistemas de monitoramento e análise de logs.

## Instalação

Instale `logger-json` usando npm:

`npm install logger-json`

Ou usando yarn:

`yarn add logger-json`

## Uso

Primeiro, importe `Logger` da `logger-json`:

    const { Logger } = require('logger-json');
    // Ou usando importações ES6  /
    / import { Logger } from 'logger-json';

Em seguida, crie uma instância do `Logger` e comece a logar:

`const logger = new Logger('info');

    logger.info('This is an info message');
    logger.debug('This is a debug message'); // Não será exibido se o nível for 'info'
    logger.warn('This is a warning message');
    logger.error('This is an error message');`

## API

### `new Logger(level)`

Cria uma nova instância do Logger.

- `level`: Define o nível de log (`info`, `debug`, `warn`, `error`). Logs abaixo desse nível não serão exibidos.

### `logger.info(message)`

Registra uma mensagem de nível `info`.

### `logger.debug(message)`

Registra uma mensagem de nível `debug`.

### `logger.warn(message)`

Registra uma mensagem de nível `warn`.

### `logger.error(message)`

Registra uma mensagem de nível `error`.

## Contribuindo

Contribuições são sempre bem-vindas! Por favor, leia o guia de contribuição para saber como você pode contribuir para o projeto.

## Licença

`logger-json` é licenciado sob a [MIT License](https://chat.openai.com/c/LICENSE).
