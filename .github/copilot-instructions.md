# Copilot Instructions for knowledge-index

## Repository Overview

This repository is an internal knowledge indexing and retrieval service demonstrating production-grade RAG (Retrieval-Augmented Generation) pipelines, data boundaries, and AI reliability safeguards.

### Project Type
- **Purpose**: Knowledge indexing and retrieval service with RAG capabilities
- **Focus Areas**: Production-grade RAG pipelines, data boundaries, AI reliability safeguards
- **Stage**: Early development/demonstration phase

## Project Structure

The repository is currently in its initial setup phase. As the project evolves, expect:
- Source code for RAG pipeline implementation
- Configuration files for AI/ML models
- Data processing and indexing components
- API endpoints for knowledge retrieval
- Security and reliability safeguards
- Documentation and examples

## Development Workflow

### Jira Integration

**IMPORTANT**: All pull requests must be linked to a Jira issue.

When creating branches, commits, and pull requests:

1. **Branch naming**: Include the Jira issue key in your branch name
   - Format: `<issue-key>-brief-description` or `<type>/<issue-key>-brief-description`
   - Example: `PROJ-123-add-rag-pipeline` or `feature/PROJ-123-add-rag-pipeline`

2. **Commit messages**: Include the Jira issue key in commit messages
   - Format: `<ISSUE-KEY>: Commit message`
   - Example: `PROJ-123: Implement vector embedding generation`

3. **Pull request titles**: Include the Jira issue key at the beginning
   - Format: `<ISSUE-KEY>: PR title`
   - Example: `PROJ-123: Add RAG pipeline implementation`

4. **Pull request descriptions**: Reference the Jira issue
   - Include a link to the Jira issue in the PR description
   - Use the format: `Jira: <ISSUE-KEY>` or include the full URL

This ensures proper tracking and integration between code changes and Jira work items.

### Getting Started

Since this is a new repository, there are no build or test commands yet. When working on this repository:

1. **Before adding new components**: Consider the production-grade requirements
   - Data boundaries and privacy considerations
   - AI reliability and safety checks
   - Scalability and performance implications

2. **When implementing RAG pipelines**: 
   - Follow best practices for vector embeddings and semantic search
   - Implement proper error handling and fallback mechanisms
   - Consider token limits and API rate limiting

3. **Security considerations**:
   - Never commit API keys, credentials, or sensitive data
   - Implement proper data sanitization for user inputs
   - Add appropriate access controls and data boundaries

### Code Quality

- Write clean, maintainable code with clear documentation
- Include type hints/annotations where applicable
- Add unit tests for new functionality
- Follow language-specific best practices for the chosen tech stack

### When Adding Dependencies

- Choose well-maintained libraries with active communities
- Consider security implications of third-party dependencies
- Document the reason for adding new dependencies
- Use lock files to ensure reproducible builds

## Best Practices for this Repository

1. **RAG Pipeline Design**: When implementing RAG components, focus on:
   - Efficient chunking strategies for knowledge documents
   - Quality embedding generation
   - Relevant context retrieval
   - Safe prompt construction

2. **Data Boundaries**: Always consider:
   - User data isolation
   - Multi-tenancy requirements
   - Data retention policies
   - Privacy-preserving techniques

3. **AI Reliability Safeguards**: Implement:
   - Input validation and sanitization
   - Output verification and filtering
   - Fallback mechanisms for model failures
   - Monitoring and observability

4. **Testing Strategy**: When tests are added, they should cover:
   - Unit tests for individual components
   - Integration tests for RAG pipeline flows
   - Security tests for data boundary enforcement
   - Performance tests for scalability

## Notes for Copilot Coding Agent

- This is a new repository in early stages - be prepared to set up foundational components
- Pay special attention to security and data privacy given the knowledge indexing nature
- When building out the project, prioritize production-grade reliability over quick prototypes
- Document architectural decisions that affect RAG pipeline design
- Consider scalability from the start, as knowledge bases can grow significantly
- Always validate that changes maintain proper data boundaries and AI safety guardrails
