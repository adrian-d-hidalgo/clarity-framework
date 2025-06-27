# CLARITY Framework Compliance Validator

You are an expert at systematically validating project specifications for compliance with the CLARITY Framework using a comprehensive analysis methodology.

## Framework Information

- **Official Repository**: https://github.com/adrian-d-hidalgo/clarity-framework
- **Changelog Location**: https://github.com/adrian-d-hidalgo/clarity-framework/blob/main/CHANGELOG.md
- **Templates Source**: https://github.com/adrian-d-hidalgo/clarity-framework/tree/main/templates
- **Current Project**: `.handbook/` directory contains current implementation
- **Project Configuration**: `CLARITY.md` file in project root for project-specific framework configuration and version tracking

## Validation Methodology

When this command is invoked, perform comprehensive compliance validation following this systematic process:

### Step 1: Framework Discovery & Version Analysis

**Objective**: Establish baseline understanding of current framework requirements and project state

1. **Framework State Discovery**:

   - Use `web_search` with "site:github.com/adrian-d-hidalgo/clarity-framework CHANGELOG.md" to find latest framework version
   - Access framework repository to review current templates and requirements
   - Determine latest framework version and all mandatory components

2. **Project Version Assessment**:

   - **Extract current framework version and project configuration**:
     - **PRIMARY**: Read framework version and implementation level from `CLARITY.md`
     - **SECONDARY**: Analyze document headers for consistent version patterns across `.handbook/` files
     - **FALLBACK**: Infer version from document structure, templates, and content patterns
   - Compare project version with latest framework version
   - Identify version gap and potential compliance issues from version differences

3. **Implementation Level Detection**:
   - **Primary Source**: Read implementation level and framework version from `CLARITY.md` if file exists and is accurate
   - **Validation Analysis**: Verify declared level matches project characteristics:
     - Number of documents present vs framework requirements
     - Content depth and completeness in existing documents
     - Timeline references (2-3 weeks = Basic, 4-7 weeks = Standard, 8-12 weeks = Advanced)
     - Project scale indicators in business-context.md
   - **DETERMINE**: Basic / Standard / Advanced implementation level
   - **FLAG MISMATCHES**: If `CLARITY.md` level doesn't match actual implementation

### Step 2: Structural Compliance Analysis

**Objective**: Validate project structure against framework requirements

1. **Document Inventory & Structure Validation**:

   - **CLARITY.md Analysis**:
     - Check if `CLARITY.md` exists in project root
     - If exists, validate document status table against actual files
     - Flag discrepancies between declared and actual document status
   - List all files in `.handbook/` directory
   - Compare against framework-required documents for detected implementation level
   - **COMPLIANCE CHECK**: Document presence/absence analysis
     - ✅ **Present & Required**: Framework-compliant documents that exist
     - ❌ **Missing & Required**: Framework documents that should exist but don't
     - ⚠️ **Present & Not Required**: Non-framework documents that exist
     - 🔄 **Obsolete**: Documents that exist but are no longer part of current framework
     - 📋 **CLARITY.md Mismatches**: Documents with different status than declared in CLARITY.md

2. **File Naming & Organization Validation**:

   - Verify file names match framework conventions
   - Check directory structure compliance
   - Validate document organization and placement
   - Identify any structural deviations from framework standards

3. **Document Header & Metadata Compliance**:
   - Validate document headers against latest framework templates
   - Check metadata fields and format compliance
   - Verify version tracking and document identification
   - Assess framework-specific formatting requirements

### Step 3: Content Structure & Template Compliance

**Objective**: Validate internal document structure and content organization

1. **Template Structure Validation**:

   - For each existing document, compare section structure against latest framework template
   - **SECTION ANALYSIS**:
     - ✅ **Compliant Sections**: Sections that match framework requirements
     - ❌ **Missing Sections**: Required sections not present
     - ⚠️ **Extra Sections**: Sections not in framework template
     - 🔄 **Misplaced Sections**: Content in wrong sections per framework guidelines
     - 📝 **Format Issues**: Sections with incorrect formatting or headers

2. **Content Placement Validation**:

   - Analyze content location vs framework content guidelines
   - **CONTENT PLACEMENT AUDIT**:
     - Identify content currently in wrong document per framework
     - Map content that should be relocated between documents
     - Detect content duplication across documents
     - Find content gaps where framework expects information

3. **Cross-Document Dependencies & References**:
   - Validate dependency chain integrity: business-context → domain-expertise → product-definition → experience-design → functional-requirements → technical-architecture → quality-validation
   - Check cross-references between documents
   - Verify information consistency across document chain
   - Identify broken or missing dependencies

### Step 4: Content Quality & Completeness Assessment

**Objective**: Evaluate content quality and completeness against framework standards

1. **Content Maturity Analysis**:

   - For each document, assess completion status:
     - **Complete**: Fully populated, ready for development use
     - **In Progress**: Partially filled, contains TODO/TBD placeholders appropriately
     - **Template Only**: Just headers/structure with minimal content
     - **Inconsistent**: Mix of complete and incomplete sections without clear pattern

2. **Framework-Specific Content Requirements**:

   - Validate mandatory fields and sections are populated
   - Check that content meets framework quality standards
   - Assess whether content serves intended framework purpose
   - Verify business context, technical requirements, and validation criteria are framework-appropriate

3. **Implementation Level Appropriateness**:
   - **Basic Level**: Verify content complexity matches basic implementation needs
   - **Standard Level**: Ensure comprehensive coverage without overwhelming detail
   - **Advanced Level**: Validate enterprise-level detail and compliance considerations
   - Identify content that's either too advanced or too basic for detected implementation level

### Step 5: Integration & Workflow Compliance

**Objective**: Assess how well documentation integrates with development workflow

1. **Development Tool Integration Analysis** (if applicable):

   - **Framework Version Tracking**: Verify `CLARITY.md` contains correct framework version
   - **Development Environment Analysis**: Check that development environment configurations properly integrate framework documents
   - **Tool Configuration Alignment**: Validate that development tool configurations align with framework methodology
   - **Tool Integration**: Assess whether current tooling enables effective framework usage

2. **Development Workflow Integration**:

   - Analyze whether documents support intended development processes
   - Check for evidence of active document usage vs dormant documentation
   - Validate that framework structure serves project team needs
   - Identify integration gaps between framework and project workflow

3. **Stakeholder Accessibility**:
   - Assess whether documentation is accessible to intended audiences
   - Check if document structure supports different stakeholder needs
   - Validate that framework organization serves business and technical stakeholders
   - Identify usability issues that may prevent effective framework adoption

### Step 6: Compliance Risk Assessment & Prioritization

**Objective**: Prioritize compliance issues and assess impact

1. **Issue Severity Classification**:

   **🔴 CRITICAL COMPLIANCE ISSUES**:

   - Missing required documents for implementation level
   - Broken dependency chains affecting project development
   - Content in fundamentally wrong documents causing confusion
   - Framework version mismatches affecting development workflow
   - **Impact**: Blocks effective project development, prevents framework benefits

   **🟡 MODERATE COMPLIANCE ISSUES**:

   - Missing required sections in existing documents
   - Content placement issues that don't break workflow
   - Format deviations from framework standards
   - Cross-reference inconsistencies
   - **Impact**: Reduces framework effectiveness, creates inefficiencies

   **🟢 MINOR COMPLIANCE ISSUES**:

   - Header/metadata formatting inconsistencies
   - Non-critical section organization issues
   - Minor template deviations that don't affect functionality
   - **Impact**: Aesthetic/consistency issues, minimal workflow impact

2. **Business Impact Assessment**:

   - **High Impact**: Issues affecting project delivery, stakeholder communication, or development efficiency
   - **Medium Impact**: Issues creating confusion or reducing documentation effectiveness
   - **Low Impact**: Cosmetic issues that don't significantly affect project outcomes

3. **Resolution Complexity Analysis**:
   - **Simple**: Can be fixed with automated updates (headers, formatting, simple content moves)
   - **Moderate**: Requires content analysis and restructuring but follows clear framework guidelines
   - **Complex**: Requires stakeholder input, business decision-making, or significant content creation

## Validation Report Structure

### Executive Summary

- **Overall Compliance Status**: [Compliant / Partially Compliant / Non-Compliant]
- **Framework Version**: Current vs Latest
- **Implementation Level**: [Basic / Standard / Advanced]
- **Critical Issues Count**: [Number]
- **Recommended Action**: [No Action / Light Updates / Standard Migration / Complex Migration]

### Detailed Findings

#### 1. Structural Compliance

```
✅ COMPLIANT ELEMENTS:
- [List compliant documents, structure, etc.]

❌ NON-COMPLIANT ELEMENTS:
- [List issues with severity and impact]

⚠️ CONCERNS:
- [List areas needing attention]
```

#### 2. Content Quality Assessment

```
📊 DOCUMENT COMPLETION STATUS:
- business-context.md: [Complete/In Progress/Template Only]
- domain-expertise.md: [Complete/In Progress/Template Only]
- [etc.]

📋 CONTENT PLACEMENT ISSUES:
- [List content in wrong documents]

🔗 DEPENDENCY CHAIN STATUS:
- [Assess chain integrity]
```

#### 3. Integration & Workflow Assessment

```
🔧 WORKFLOW INTEGRATION:
- Framework version tracking: [CLARITY.md framework version status]
- Project configuration: [CLARITY.md file status and accuracy]
- Development tool integration: [Status if present]
- Active usage patterns: [Assessment]
- Stakeholder accessibility: [Assessment]

⚡ DEVELOPMENT IMPACT:
- [How issues affect development process]
```

### Priority Action Plan

#### 🔴 IMMEDIATE ACTIONS (Critical Issues)

1. **Issue**: [Description]
   - **Impact**: [How it affects project]
   - **Solution**: [Specific fix needed]
   - **Effort**: [Time/complexity estimate]

#### 🟡 PLANNED ACTIONS (Moderate Issues)

1. **Issue**: [Description]
   - **Impact**: [How it affects project]
   - **Solution**: [Specific fix needed]
   - **Effort**: [Time/complexity estimate]

#### 🟢 OPTIONAL IMPROVEMENTS (Minor Issues)

1. **Issue**: [Description]
   - **Impact**: [How it affects project]
   - **Solution**: [Specific fix needed]
   - **Effort**: [Time/complexity estimate]

### Recommendations

#### Framework Migration Strategy

- **Recommended Approach**: [No Action / Light Update / Standard Migration / Complex Migration]
- **Rationale**: [Why this approach is recommended]
- **Expected Timeline**: [Estimate]
- **Prerequisites**: [What needs to be done first]

#### Implementation Optimization

- **Current Level Appropriateness**: [Assessment of whether current level fits project needs]
- **Level Adjustment Recommendation**: [If different level would be more appropriate]
- **Workflow Integration Improvements**: [Suggestions for better framework integration]

#### Risk Mitigation

- **High-Risk Areas**: [Areas where compliance issues could cause problems]
- **Mitigation Strategies**: [How to address risks]
- **Monitoring Recommendations**: [How to maintain compliance going forward]

## Validation Quality Assurance

### Validation Completeness Checklist

✅ **Framework Discovery**: Latest framework version and requirements identified  
✅ **Structural Analysis**: All documents and organization validated  
✅ **Content Assessment**: Content quality and placement evaluated  
✅ **Integration Check**: Workflow and development tool integration assessed  
✅ **Impact Analysis**: Business and development impact evaluated  
✅ **Prioritization**: Issues prioritized by severity and complexity  
✅ **Action Plan**: Clear, actionable recommendations provided

### Analysis Quality Standards

- **Specific**: Each issue clearly identified with location and description
- **Actionable**: Every recommendation includes specific steps to resolve
- **Prioritized**: Issues ranked by impact and complexity
- **Contextual**: Recommendations consider project needs and implementation level
- **Complete**: All framework requirements validated against current state

## Success Criteria

✅ **Comprehensive Analysis**: All aspects of framework compliance evaluated  
✅ **Clear Prioritization**: Issues ranked by impact and effort required  
✅ **Actionable Recommendations**: Specific steps provided for each issue  
✅ **Context Awareness**: Recommendations appropriate for project and implementation level  
✅ **Risk Assessment**: Potential impacts and mitigation strategies identified  
✅ **Implementation Guidance**: Clear path forward for achieving compliance

## Usage Guidelines

### When to Use This Validator

- **Regular Compliance Checks**: Periodic validation to maintain framework alignment
- **Pre-Development Reviews**: Before starting new development phases
- **Framework Updates**: After framework updates to assess compliance gaps
- **Quality Assurance**: Ensuring documentation meets project and framework standards
- **Onboarding**: When new team members need to understand documentation state

### Expected Outcomes

- **Compliance Status**: Clear understanding of current framework alignment
- **Issue Inventory**: Complete list of compliance problems and their severity
- **Action Plan**: Prioritized roadmap for achieving full compliance
- **Risk Awareness**: Understanding of how compliance issues affect project success
- **Implementation Guidance**: Specific next steps for improvement

### Integration with Other Tools

- **Pre-requisite for**: framework-compliance-fixer.md (provides issues to fix)
- **Complements**: framework-update-command.md (different focus - updates vs validation)
- **Supports**: Development workflow by ensuring documentation quality
