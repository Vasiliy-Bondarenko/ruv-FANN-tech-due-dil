# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a technical due diligence analysis repository focused on evaluating the ruv-FANN neural network project. The repository contains comprehensive assessments of implementation quality, security vulnerabilities, and business viability claims.

## Repository Structure

The repository is organized into two main areas:

### Assessment Reports (`assessments/`)
Contains detailed technical analysis reports:
- `critical-security-assessment.md` - Security vulnerability analysis
- `implementation-verification-summary.md` - Code implementation quality review
- etc

### Executive Summary
- `executive-summary*.md` - Comprehensive business and technical assessment

## Key Project Characteristics

### Analysis Focus Areas
1. **Implementation Quality**: Code verification, functionality testing, and architecture assessment
2. **Security Analysis**: Supply chain vulnerabilities, permission bypasses, and attack vectors
3. **Business Viability**: Marketing claims vs. implementation reality
4. **Compatibility Assessment**: API compatibility with claimed libraries (NeuralForecast, FANN)
5. **Maintainer Response**: Issue handling and transparency evaluation

### Assessment Methodology
- **Evidence-Based**: Every claim must link to specific code files/lines with GitHub commit references
- **Verifiable**: All findings include reproducible verification steps
- **Professional**: Suitable for board-level presentation to investors and CTOs
- **Honest**: Acknowledges both strengths and critical gaps without bias

## Working with This Repository

### Reading Assessment Reports
- All reports include specific commit hashes for GitHub links
- Line numbers are provided for exact code references
- Findings are categorized by severity (CRITICAL, HIGH, MEDIUM, LOW)
- Each report includes verification steps for independent confirmation

### Adding New Assessments
- Follow the standard header format with date, repository link, and commit hash
- Include concrete technical details and avoid speculation
- Provide implementation-level specifics with exact code quotes
- Never use "we", "our", "us" - maintain individual assessment perspective

### Evidence Standards
- Link to specific GitHub files with commit hashes
- Quote exact text from README and code files
- Provide verifiable percentages and metrics
- No assumptions or speculation without explicit disclaimer

## Important Notes

### Forbidden Content
- ❌ Recommendations or advice to project owners
- ❌ Development timelines or resource estimates
- ❌ Strategic guidance for stakeholders
- ❌ Methodology disclosure or due diligence process explanation

### Link Requirements
- All GitHub links must include specific commit hash
- Reference exact line numbers where possible
- Ensure all links are verifiable and permanent

### Assessment Quality Markers
All outputs should be:
- **Comprehensive**: Covers all relevant aspects
- **Verifiable**: Every finding links to specific evidence
- **Professional**: Suitable for board-level presentation
- **Honest**: Acknowledges both strengths and critical gaps
- **Actionable**: Provides clear risk assessment for decisions

## File Naming Convention

Assessment files follow the pattern: `[topic]-[type]-[assessment|report|analysis].md`

Examples:
- `critical-security-assessment.md`
- `implementation-verification-summary.md`
- `neuralforecast-compatibility-assessment.md`