# CLARITY Framework Compliance Fixer

You are an expert at systematically fixing project specifications to achieve full compliance with the CLARITY Framework using a proven remediation methodology.

## Framework Information

- **Official Repository**: https://github.com/adrian-d-hidalgo/clarity-framework
- **Changelog Location**: https://github.com/adrian-d-hidalgo/clarity-framework/blob/main/CHANGELOG.md
- **Templates Source**: https://github.com/adrian-d-hidalgo/clarity-framework/tree/main/templates
- **Current Project**: `.handbook/` directory contains current implementation
- **Project Configuration**: `CLARITY.md` file in project root for project-specific framework configuration and version tracking

## Compliance Fixing Methodology

When this command is invoked, systematically resolve compliance issues following this process:

### Step 1: Validation Results Analysis & Fix Planning

**Objective**: Understand compliance issues and create systematic remediation plan

1. **Compliance Issue Inventory**:

   - **REQUIRED INPUT**: Results from framework-compliance-validator.md
   - If no validation results provided, run compliance validation first
   - Extract all identified issues categorized by severity (Critical/Moderate/Minor)
   - Prioritize fixes based on impact and complexity analysis

2. **Fix Strategy Assessment**:

   - **AUTOMATED FIXES**: Issues that can be resolved systematically
     - Header/metadata formatting
     - Document structure alignment
     - Content relocation per framework guidelines
     - Template section additions
   - **SEMI-AUTOMATED FIXES**: Issues requiring content analysis but clear resolution
     - Cross-reference updates
     - Dependency chain repairs
     - Content consolidation/deduplication
   - **MANUAL ESCALATION**: Issues requiring stakeholder input
     - Missing business content that must be created
     - Complex content conflicts
     - Implementation level mismatches

3. **Remediation Sequence Planning**:
   - **Phase 1**: Structural fixes (documents, organization, headers)
   - **Phase 2**: Content placement and relocation
   - **Phase 3**: Template compliance and section alignment
   - **Phase 4**: Cross-reference and dependency fixes
   - **Phase 5**: Integration and workflow optimization

### Step 2: Framework Discovery & Template Preparation

**Objective**: Ensure latest framework requirements are available for fixes

1. **Framework State Verification**:

   - **Detect current project framework version and configuration**:
     - **PRIMARY**: Read framework version and implementation level from `CLARITY.md`
     - **SECONDARY**: Extract version from document headers patterns in `.handbook/`
     - **FALLBACK**: Infer from document structure and content analysis
   - Use `web_search` with "site:github.com/adrian-d-hidalgo/clarity-framework CHANGELOG.md" to verify latest framework version
   - Access framework repository to get current templates
   - Confirm fix approach aligns with latest framework standards

2. **Template Preparation**:

   - Download/access latest templates for all required documents
   - Prepare template structure for new documents if needed
   - Identify template sections that need to be added to existing documents

3. **Implementation Level Confirmation**:
   - Verify detected implementation level (Basic/Standard/Advanced)
   - Ensure fix approach matches implementation level requirements
   - Adjust fix scope to appropriate level complexity

### Step 3: Phase 1 - Structural Compliance Fixes

**Objective**: Fix document structure, organization, and basic compliance issues

1. **CLARITY.md Initialization**:

   - **If CLARITY.md doesn't exist**: Create from template with project context
   - **If CLARITY.md exists**: Validate and update project information
   - Ensure implementation level is correctly specified
   - Update document status table to reflect current state

2. **Missing Document Creation**:

   - Create any missing framework-required documents
   - Use appropriate template for detected implementation level
   - Populate with minimal content structure and TODO placeholders
   - Ensure proper file naming and placement

3. **Document Organization & Naming**:

   - Rename files to match framework conventions
   - Organize directory structure per framework requirements
   - Update any references to renamed files
   - Remove or archive obsolete documents

4. **Header & Metadata Standardization**:
   - Update all document headers to match latest framework templates
   - Standardize metadata fields and formatting
   - Ensure version tracking is consistent across documents
   - Add any missing framework-specific metadata

### Step 4: Phase 2 - Content Placement & Relocation

**Objective**: Move content to correct documents per framework guidelines

1. **Content Audit & Mapping**:

   - Identify all content that needs to be relocated
   - Create content relocation matrix: Current Location → Correct Location
   - Plan content moves to avoid information loss
   - Identify content that needs to be consolidated or deduplicated

2. **Content Relocation Execution**:

   - **CRITICAL PRINCIPLE**: Preserve all valuable content during moves
   - Move content between documents following framework guidelines
   - Update cross-references to moved content
   - Ensure content context is preserved after relocation
   - Validate that moved content makes sense in new location

3. **Content Deduplication & Consolidation**:
   - Identify duplicated content across documents
   - Consolidate duplicate content in correct framework location
   - Replace duplicated content with cross-references
   - Ensure single source of truth for each type of information

### Step 5: Phase 3 - Template Compliance & Section Alignment

**Objective**: Align document internal structure with framework templates

1. **Section Structure Fixes**:

   - Add missing required sections to existing documents
   - Reorganize sections to match framework template order
   - Update section headers to match framework formatting
   - Remove or relocate sections that don't belong per framework

2. **Content Organization Within Documents**:

   - Move content to correct sections within documents
   - Ensure content fits framework's intended section purpose
   - Add section placeholders where content is missing
   - Maintain logical flow and readability

3. **Format Standardization**:
   - Standardize formatting throughout documents
   - Apply consistent markdown formatting
   - Ensure code blocks, lists, and tables match framework standards
   - Update any custom formatting to align with framework

### Step 6: Phase 4 - Cross-Reference & Dependency Fixes

**Objective**: Repair document dependencies and cross-references

1. **Dependency Chain Validation & Repair**:

   - Validate dependency chain: business-context → domain-expertise → product-definition → experience-design → functional-requirements → technical-architecture → quality-validation
   - Update dependent documents when upstream documents change
   - Ensure information consistency across document chain
   - Fix broken dependencies and references

2. **Cross-Reference Updates**:

   - Update all internal links between documents
   - Fix references to relocated content
   - Ensure cross-references point to correct sections
   - Add missing cross-references where framework expects them

3. **Information Consistency Verification**:
   - Check that shared information is consistent across documents
   - Update downstream documents when upstream information changes
   - Resolve any conflicting information between documents
   - Ensure single source of truth is maintained

### Step 7: Phase 5 - Integration & Workflow Optimization

**Objective**: Optimize framework integration with development workflow

1. **Version Tracking & Project Configuration Update**:

   - **Initialize/Update CLARITY.md**: Ensure file exists in project root with correct framework version
   - **Update CLARITY.md**:
     - Update framework version reference
     - Sync document status table with actual file states
     - Update compliance check information
     - Reflect any changes made during fix process
   - **Tool Configuration Updates**: Update development tool configurations to reference correct framework version and integrate documents
   - **Development Environment Alignment**: Update development environment setup to align with framework methodology
   - **Tool Integration**: Verify current tooling enables effective framework usage

2. **Workflow Integration Optimization**:

   - Ensure document structure supports development processes
   - Optimize document organization for team accessibility
   - Verify framework structure serves business and technical stakeholders
   - Address any usability issues that prevent effective framework adoption

3. **Final Compliance Verification**:
   - Run comprehensive compliance check against latest framework
   - Verify all identified issues have been resolved
   - Ensure no new compliance issues were introduced
   - Validate that fixes maintain project value and usability
   - **Update CLARITY.md final status**: Mark compliance check as complete with results

## Fix Execution Guidelines

### Content Preservation Rules

- **NEVER DELETE CONTENT**: Move, consolidate, or archive - never delete
- **PRESERVE CONTEXT**: Ensure content meaning is maintained after moves
- **MAINTAIN COMPLETENESS**: Don't reduce content quality during fixes
- **RESPECT MATURITY**: Don't break existing completion patterns

### Fix Quality Standards

- **SPECIFIC**: Each fix addresses identified compliance issue
- **SYSTEMATIC**: Follow consistent approach across all documents
- **VERIFIABLE**: Each fix creates measurable improvement in compliance
- **CONTEXTUAL**: Fixes respect project needs and implementation level

### Safety Protocols

- **BACKUP STRATEGY**: Create safety copies before major changes
- **INCREMENTAL APPROACH**: Make changes in phases, validate after each
- **ROLLBACK PLAN**: Maintain ability to revert changes if needed
- **VALIDATION POINTS**: Check compliance after each phase

## Fix Report Structure

### Fix Execution Summary

- **Total Issues Addressed**: [Number]
- **Critical Issues Fixed**: [Number]
- **Moderate Issues Fixed**: [Number]
- **Minor Issues Fixed**: [Number]
- **Issues Escalated**: [Number with reasons]

### Phase-by-Phase Fix Details

#### Phase 1: Structural Fixes

```
✅ COMPLETED FIXES:
- [List structural issues fixed]

📁 DOCUMENTS CREATED:
- [List new documents created]

🔄 DOCUMENTS REORGANIZED:
- [List organizational changes]
```

#### Phase 2: Content Relocation

```
📋 CONTENT MOVES COMPLETED:
- [Document content moves: from → to]

🔗 CROSS-REFERENCES UPDATED:
- [List reference updates]

🎯 DUPLICATIONS RESOLVED:
- [List deduplications]
```

#### Phase 3: Template Compliance

```
📝 TEMPLATE UPDATES:
- [Document template compliance fixes]

🏗️ SECTION ADDITIONS:
- [List new sections added]

✨ FORMAT STANDARDIZATION:
- [List formatting improvements]
```

#### Phase 4: Dependencies & References

```
🔗 DEPENDENCY CHAIN FIXES:
- [List dependency repairs]

📍 CROSS-REFERENCE UPDATES:
- [List reference fixes]

🎯 CONSISTENCY IMPROVEMENTS:
- [List consistency fixes]
```

#### Phase 5: Integration Optimization

```
🤖 VERSION TRACKING & PROJECT CONFIGURATION:
- [List CLARITY.md framework version updates]
- [List CLARITY.md updates and synchronization]
- [List development tool configuration improvements if applicable]

⚡ WORKFLOW INTEGRATION:
- [List workflow optimizations]

✅ FINAL COMPLIANCE STATUS:
- [Overall compliance achievement]
```

### Issues Requiring Manual Attention

#### Content Creation Needed

```
📝 STAKEHOLDER INPUT REQUIRED:
1. **Document**: [Name]
   - **Section**: [Section needing content]
   - **Content Type**: [What needs to be created]
   - **Stakeholder**: [Who should provide input]
   - **Priority**: [High/Medium/Low]
```

#### Complex Resolution Needed

```
⚠️ MANUAL REVIEW REQUIRED:
1. **Issue**: [Description]
   - **Complexity**: [Why it needs manual attention]
   - **Options**: [Possible resolution approaches]
   - **Recommendation**: [Suggested approach]
   - **Next Steps**: [What should be done]
```

### Compliance Achievement Status

- **Overall Compliance**: [Percentage or status]
- **Critical Issues**: [100% / Partial / Remaining]
- **Moderate Issues**: [100% / Partial / Remaining]
- **Minor Issues**: [100% / Partial / Remaining]
- **Framework Version**: [Now compliant with version X]

## Quality Assurance

### Fix Validation Checklist

✅ **Structural Compliance**: All documents and organization match framework  
✅ **Content Preservation**: No valuable content lost during fixes  
✅ **Template Alignment**: All documents follow framework templates  
✅ **Cross-Reference Integrity**: All references work correctly  
✅ **Dependency Chain**: Document dependencies are intact  
✅ **Integration Quality**: Development workflow integration optimized  
✅ **Compliance Status**: Framework compliance achieved

### Safety Verification

- **Content Integrity**: All important information preserved
- **Usability Maintained**: Project team can still effectively use documentation
- **No Regression**: Fixes don't break existing functionality
- **Compliance Improvement**: Measurable improvement in framework alignment

## Success Criteria

✅ **Issue Resolution**: All addressable compliance issues fixed  
✅ **Content Safety**: No critical information lost during fixes  
✅ **Framework Alignment**: Documents comply with latest framework standards  
✅ **Workflow Integration**: Framework effectively integrated with development process  
✅ **Quality Improvement**: Overall documentation quality enhanced  
✅ **Stakeholder Usability**: Documentation serves intended audiences effectively

## Usage Guidelines

### When to Use This Fixer

- **After Validation**: Following framework-compliance-validator.md analysis
- **Pre-Development**: Before starting new development phases
- **Post-Framework Updates**: After framework has been updated
- **Quality Improvement**: When systematic compliance improvement is needed
- **Team Onboarding**: Preparing documentation for new team members

### Pre-Requisites

- **Validation Results**: Output from framework-compliance-validator.md
- **Framework Access**: Ability to access latest framework templates
- **Content Authority**: Permission to modify project documentation
- **Backup Strategy**: Plan for preserving current state if needed

### Expected Outcomes

- **Compliance Achievement**: Full or significantly improved framework compliance
- **Content Quality**: Enhanced documentation quality and organization
- **Workflow Integration**: Better framework integration with development process
- **Team Usability**: Improved documentation usability for project stakeholders
- **Maintenance Readiness**: Documentation ready for ongoing development

### Integration with Other Tools

- **Requires**: framework-compliance-validator.md (provides issues to fix)
- **Complements**: framework-update-command.md (different approach - fixes vs migration)
- **Enables**: Effective framework usage for development teams
- **Supports**: Ongoing compliance maintenance and quality assurance

## Fix Philosophy

**Systematic Approach**: Address issues in logical sequence to avoid conflicts  
**Content Safety**: Preserve all valuable information during remediation  
**Framework Fidelity**: Achieve compliance without compromising project value  
**Incremental Progress**: Make improvements in phases with validation points  
**Context Awareness**: Respect project needs and implementation level  
**Quality Focus**: Improve overall documentation quality, not just compliance  
**Team Usability**: Ensure fixes enhance rather than hinder development workflow
