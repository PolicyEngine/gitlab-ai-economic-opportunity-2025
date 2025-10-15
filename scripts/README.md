# Scripts

Utility scripts for managing the grant application.

## Available Scripts

### `assemble_concept_note.py` (to be created)
Assembles individual response files into a complete concept note document.

Usage:
```bash
cd docs/concept-note
python3 assemble_concept_note.py
```

### `validate_word_counts.py` (to be created)
Validates that all responses meet word count requirements.

Usage:
```bash
python3 scripts/validate_word_counts.py
```

### `sync_content.py` (to be created)
Syncs content between markdown files and any review site (if applicable).

Usage:
```bash
python3 scripts/sync_content.py
```

## Creating New Scripts

When creating scripts:

1. **Use Python 3**: Ensure compatibility with Python 3.8+
2. **Document Usage**: Include docstrings and usage examples
3. **Handle Errors**: Gracefully handle missing files or malformed input
4. **Validate Output**: Check that generated files are correct
5. **Make Executable**: Set appropriate permissions (`chmod +x script.py`)

## Common Patterns

### Reading Response Files
```python
import os
from pathlib import Path

responses_dir = Path("docs/concept-note/responses")
response_files = sorted(responses_dir.glob("*.md"))

for file in response_files:
    with open(file, 'r') as f:
        content = f.read()
        # Process content
```

### Word Counting
```python
def count_words(text):
    """Count words in text, excluding markdown headers and comments."""
    # Remove markdown headers
    text = re.sub(r'^#.*$', '', text, flags=re.MULTILINE)
    # Remove HTML comments
    text = re.sub(r'<!--.*?-->', '', text, flags=re.DOTALL)
    # Count words
    return len(text.split())
```

### Assembling Documents
```python
def assemble_document(response_files, output_file):
    """Assemble multiple response files into single document."""
    with open(output_file, 'w') as out:
        for file in response_files:
            with open(file, 'r') as f:
                out.write(f.read())
                out.write('\n\n---\n\n')
```

## Future Enhancements

Potential scripts to add:
- Export to PDF for submission
- Generate budget tables from structured data
- Check for required sections
- Lint markdown files
- Generate executive summary
- Create submission checklist
