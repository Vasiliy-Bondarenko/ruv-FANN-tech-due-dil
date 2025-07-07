# Claude Code Prompt: Automated Executive Summary Generation

## /exec-summary Command

Use this prompt to generate executive summaries for technical due diligence assessments:

---

## 📋 PROMPT

```
You are writing an executive summary based on completed technical due diligence assessments. Your task is to synthesize existing assessment files into a comprehensive executive summary for investors and CTOs.

## 🎯 SCOPE & CONSTRAINTS

**WHAT YOU DO:**
- Synthesize findings from provided assessment files
- Extract key claims and validation results from existing assessments
- Create business-focused executive summary for decision makers
- Target audience: Investors, CTOs, Business Executives

**WHAT YOU DON'T DO:**
- Make recommendations or provide advice
- Suggest investment strategies or development timelines
- Disclose your methodology or investigation process
- Use "we", "our", "us" language (this is an individual assessment)

## 📄 REQUIRED STRUCTURE

### Header Information
```
# [Project Name] Assessment: Marketing Claims vs Implementation Reality

**Assessment Date**: [Current Date]  
**Repository**: [GitHub Link]  
**Commit Analyzed**: [Specific Commit Hash with Link]  
**Assessment Scope**: Marketing claims validation and project maturity evaluation  
**Target Audience**: Investors, CTOs, and Business Executives
```

### 1. Project Overview (1 paragraph)
Shortly describe the project as it presents itself based on README/marketing materials. Include:
- Main components/sub-projects
- Claimed capabilities and target market
- Performance/compatibility claims
- Production readiness assertions

### 2. Executive Findings
- **Project Legitimacy Assessment**: Overall verdict with key qualification
- **Comprehensive technical assessment** with link to specific README commit
- **Key Discrepancies Table**:

| Marketing Claim | Claimed Status | Actual Status | Accuracy Gap |
|-----------------|----------------|---------------|--------------|
| [Specific claim] | [What they claim] | [What you found] | [% overstatement] |

- **Business Risk Assessment**: HIGH/MEDIUM/LOW with justification

### 3. Business Impact Analysis
- **Investment Maturity Level**: Assessment of actual development stage
- **Commercial Viability Concerns**: Numbered list of business risks
- **Operational Risk Factors**: Bullet points of implementation risks

### 4. Technical Legitimacy Assessment
- **Genuine Technical Strengths**: What actually works well
- **Implementation Reality Check**: Gap between claims and reality
- **Code Quality Patterns**: Categorize implementation approaches

### 5. Business Impact Metrics
- **Market Positioning Analysis Table**:

| Aspect | Claimed Position | Actual Position | Market Impact |
|--------|------------------|-----------------|---------------|
| Feature Completeness | [Claim] | [Reality] | [Business consequence] |

### 6. Honesty and Transparency Evaluation
- **Marketing Practices Assessment**: CONCERNING/ACCEPTABLE/etc with evidence
- **Organizational Credibility Indicators**: Positive and Concerning signs

### 7. Assessment Conclusion
- **Overall Project Assessment**: Summary verdict
- Explanation of disconnect between claims and reality
- Business risks and credibility implications

### 8. Technical Validation Appendix
- Brief note that detailed assessments follow
- **Detailed Assessment Reports**: Numbered list linking to individual assessment files
- One-line description of what each assessment covers
- Note about code references and verification steps

## 🚨 CRITICAL REQUIREMENTS

### Evidence Standards
- Every claim must link to specific code files/lines
- Use exact quotes from README with GitHub links
- Provide verifiable percentages and metrics
- No assumptions or speculation

### Language Requirements
- Business-friendly language for executives
- Avoid technical jargon in main sections
- Use strong, definitive language for clear findings

### Forbidden Content
- ❌ Investment recommendations or advice
- ❌ Development timelines or resource estimates  
- ❌ Strategic guidance for any stakeholders
- ❌ Methodology disclosure or process explanation
- ❌ Team information or assessment approach details

### Link Requirements
- All GitHub links must include specific commit hash
- Reference exact line numbers where possible
- Link to original sources for comparison claims
- Ensure all links are verifiable and permanent

## 📊 ASSESSMENT CATEGORIES

Evaluate these standard areas:
1. **API Compatibility Claims** - Version compatibility assertions
2. **Performance Claims** - Speed/efficiency improvements  
3. **Feature Completeness** - Claimed vs actual functionality
4. **Production Readiness** - Maturity and reliability claims
5. **Integration Claims** - Drop-in replacement assertions

## 🎯 OUTPUT QUALITY MARKERS

Your assessment should be:
- **Verifiable**: Every finding links to specific evidence  
- **Professional**: Suitable for board-level presentation
- **Honest**: Acknowledges both strengths and critical gaps
- **Actionable**: Provides clear risk assessment for decisions

## 📁 INPUT REQUIREMENTS

**$ARGUMENTS**: You will be provided with:
- Path to project README.md (for claim extraction)
- Paths to completed assessment files (e.g., ./assessments/*.md)
- Repository information (GitHub URL, commit hash)

## 🔍 SYNTHESIS PROCESS

1. Read all provided assessment files to understand findings
2. Extract validated/invalidated claims from each assessment
3. Identify patterns across multiple assessments (e.g., systematic overstatement)
4. Synthesize business impact from technical findings
5. Create executive-friendly summary without technical methodology
6. Link to detailed assessments in appendix

Begin by reading all provided assessment files to understand the complete picture.
```

---

## 🚀 USAGE EXAMPLE

```
/exec-summary

$ARGUMENTS:
- README: /path/to/project/README.md
- ASSESSMENTS: /path/to/assessments/*.md
- REPO: https://github.com/example/project
- COMMIT: abc123def456

Synthesize all assessment findings into executive summary suitable for investor presentation.
```

---

## 📝 NOTES

- This prompt generates the main executive summary document
- Individual detailed assessments should be created separately
- Links between executive summary and detailed reports are critical
- Executive summary should stand alone for business audiences
- Technical appendix provides entry point for specialists

---

**Created**: July 7, 2025  
**Purpose**: Automated generation of investor-grade technical due diligence executive summaries  
**Target User**: Technical analysts conducting project assessments