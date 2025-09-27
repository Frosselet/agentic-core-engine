# Claude Code Configuration - Core Engine

## Project: Agentic Core Engine
Domain models and base infrastructure for the agentic data scraper ecosystem.

### Scope
This repository contains the core domain models and base classes:
- Base agent framework
- Security infrastructure
- Core domain models
- Shared utilities and interfaces

### Key Files
- `src/agentic_core/base_agent.py` - Abstract base agent class
- `src/agentic_core/security/` - Security and authentication modules

### Development Standards
- Follow SOLID principles and clean architecture
- All agents must inherit from BaseAgent
- Implement proper typing with Pydantic models
- Security-first design patterns
- Comprehensive unit testing required

### Cross-Repository Dependencies
- **Depends On**: `agentic-semantic-ontologies` for ontology validation
- **Used By**: `agentic-baml-agents`, `agentic-data-collectors`, `agentic-business-contracts`
- **Related**: All other repositories use these core models

### Key Commands
```bash
# Run core tests
python -m pytest src/agentic_core/tests/

# Type checking
mypy src/agentic_core/

# Security validation
python -m agentic_core.security.validator
```

### Architecture Notes
This is the foundational layer that all other services depend on. Changes here impact the entire ecosystem.