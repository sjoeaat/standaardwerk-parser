# Standaardwerk Parser

Core parsing engine for converting industrial step programs from Word documents to structured data formats.

## Features

- **Multi-format Input**: Parse DOCX files with industrial step programs
- **Advanced Parsing**: Support for RUST/SCHRITT methodology
- **Flexible Output**: JSON and XML export formats
- **Validation**: Built-in syntax and logic validation
- **CLI Tools**: Command-line interface for batch processing

## Installation

```bash
npm install
```

## Usage

### CLI Usage

```bash
# Parse a DOCX file
node cli/parser.js input.docx output.json

# Convert DOCX to JSON
node cli/docx-to-json.js input.docx
```

### Programmatic Usage

```javascript
import { AdvancedParser } from './src/core/AdvancedParser.js';
import { syntaxRules } from './src/config/syntaxRules.js';

const parser = new AdvancedParser(syntaxRules);
const result = await parser.parseDocument(documentContent);
```

## Configuration

- `src/config/syntaxRules.js` - Syntax recognition rules
- `src/config/validationRules.js` - Validation rules

## Testing

```bash
# Run unit tests
npm test

# Run specific test
node tests/unit/test-advanced-parser.js
```

## Documentation

See `docs/` directory for detailed documentation.

## Related Projects

- **standaardwerk-trainer** - Training and pattern generation
- **standaardwerk-webapp** - Web interface
- **standaardwerk-archive** - Historical data and debug tools

## License

MIT