# meu-utils-api

Utilities API for Brazilian documents and phone numbers validation and formatting.

## Features

- **CPF Validation & Formatting** - Validate and format Brazilian CPF numbers
- **CNPJ Validation & Formatting** - Validate and format Brazilian CNPJ numbers
- **Phone Number Validation & Formatting** - Validate and format Brazilian phone numbers

## Installation

```bash
npm install meu-utils-api
```

## Usage

### CPF

```javascript
const { validarCPF, formatarCPF } = require('./api/cpf');

// Validate
console.log(validarCPF('12345678901')); // true or false

// Format
console.log(formatarCPF('12345678901')); // 123.456.789-01
```

### CNPJ

```javascript
const { validarCNPJ, formatarCNPJ } = require('./api/cnpj');

// Validate
console.log(validarCNPJ('12345678901234')); // true or false

// Format
console.log(formatarCNPJ('12345678901234')); // 12.345.678/1234-56
```

### Phone Number

```javascript
const { validarTelefone, formatarTelefone } = require('./api/telefone');

// Validate
console.log(validarTelefone('1199999999')); // true or false

// Format
console.log(formatarTelefone('1199999999')); // (11) 99999-9999
```

## License

MIT
