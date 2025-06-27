# CLARITY Framework Update Command

You are an expert at systematically updating project specifications to comply with any version of the CLARITY Framework using a proven step-by-step methodology.

## Framework Information

- **Official Repository**: https://github.com/adrian-d-hidalgo/clarity-framework
- **Changelog Location**: https://github.com/adrian-d-hidalgo/clarity-framework/blob/main/CHANGELOG.md
- **Templates Source**: https://github.com/adrian-d-hidalgo/clarity-framework/tree/main/templates
- **Current Project**: `.handbook/` directory contains current implementation

## Methodology

When this command is invoked, follow this systematic process that works for ANY framework version update:

### Step 1: Migration Scope Assessment

**Objective**: Determine if migration is needed and what type of update is required

1. **Update Necessity Evaluation**:

   - Compare current project version with latest framework version
   - Assess scope of changes: Minor (patch) / Moderate (structure) / Major (breaking changes)
   - **DECISION POINT**: Determine migration type needed:
     - **No Action**: Only documentation updates, no structural changes
     - **Light Update**: Minor formatting, headers, or metadata changes
     - **Standard Migration**: Content relocation, new sections, dependency updates
     - **Complex Migration**: Breaking changes, new/obsolete documents, major restructuring
     - **Manual Escalation**: Changes too complex for automated migration

2. **Special Conditions Detection**:

   - **New Documents**: Framework requires documents that don't exist in project
   - **Obsolete Documents**: Framework no longer includes documents that exist in project
   - **Version Jump**: Multiple version changes requiring sequential migration
   - **Breaking Changes**: Framework changes that conflict with existing project structure
   - **Custom Modifications**: Project has custom additions that may conflict with framework updates

### Step 2: Framework Discovery & Gap Analysis

**Objective**: Understand specific changes and conflicts between versions

1. **Current State Assessment & Project Context Analysis**:

   **A. Implementation Level Detection**:

   - Identify current framework implementation level (Basic/Standard/Advanced) by analyzing:
     - Number of documents present vs framework requirements
     - Depth and completeness of existing content
     - Project scope indicators in business-context.md
     - Timeline references (2-3 weeks = Basic, 4-7 weeks = Standard, 8-12 weeks = Advanced)

   **B. Document Completeness Analysis**:

   - For each existing document, assess completion status:
     - **Complete**: Fully populated, ready for development
     - **In Progress**: Partially filled, contains TODO/TBD placeholders
     - **Template Only**: Just headers/structure with minimal content
     - **Customized**: Contains project-specific modifications beyond standard framework

   **C. Usage Pattern Assessment**:

   - Analyze `CLAUDE.md` or project README to understand which documents are actively referenced
   - Check for evidence of documents being used in development workflow
   - Identify documents that exist but may not be integrated into project workflow
   - Look for custom files or sections that indicate specialized project needs

   **D. Project Maturity & Context**:

   - Determine project phase: Planning / Specification / Development / Production
   - Identify business domain and any regulatory/compliance requirements
   - Assess team structure based on document ownership patterns
   - Check for integration with external tools or systems mentioned in documentation

   **E. Current Framework Version & Customizations**:

   - Extract current framework version from document headers, CLAUDE.md, or metadata
   - List all files in `.handbook/` directory structure
   - Identify any non-standard files or custom additions
   - Document any framework template modifications or extensions
   - Note any project-specific naming conventions or organizational patterns

2. **Framework State Discovery**:

   - Use `web_search` with "site:github.com/adrian-d-hidalgo/clarity-framework CHANGELOG.md" to find latest changes
   - Access framework repository directly to review current templates
   - Focus on CHANGELOG.md to understand all changes since project's current version

3. **Context-Aware Gap Analysis**:

   **A. Framework Compliance Gap Analysis**:

   - List every difference between current project structure and latest framework requirements
   - Identify changed document headers, sections, metadata formats
   - Note new/removed/modified sections in templates
   - **CONTENT PLACEMENT RULES**: Document which types of content belong in which documents per new framework
   - **CONTENT MIGRATION MATRIX**: Map current content location → correct framework location
   - Document file naming or location changes required
   - Map cross-document dependency changes
   - Record any new mandatory fields or sections

   **B. Implementation Level Considerations**:

   - **For Basic Level Projects**: Focus on core documents only, avoid overwhelming with advanced sections
   - **For Standard Level Projects**: Include all standard framework documents and sections
   - **For Advanced Level Projects**: Ensure enterprise-level sections and compliance requirements are addressed
   - Match migration scope to current project implementation level - don't force higher levels unless explicitly needed

   **C. Content Maturity-Based Migration Strategy**:

   - **Complete Documents**: Full migration with content preservation as top priority
   - **In Progress Documents**: Migrate structure while preserving existing work and maintaining TODO placeholders
   - **Template Only Documents**: Simple template updates, maintain minimal content approach
   - **Customized Documents**: Preserve customizations while ensuring framework compliance

   **D. Usage Pattern-Informed Prioritization**:

   - Prioritize migration of actively used documents over dormant ones
   - Maintain current workflow patterns unless framework changes require modification
   - Preserve tool integrations and external references
   - Consider impact on development team's current processes

### Step 3: Special Case Handling & Escalation

**Objective**: Handle edge cases and complex scenarios before proceeding with standard migration

1. **Escalation Decision Matrix**:

   **PROCEED WITH STANDARD MIGRATION** when:

   - Changes are structural but straightforward (new sections, metadata updates, content relocation)
   - Framework updates are additive (no breaking changes)
   - No conflicts between existing content and new requirements

   **ESCALATE TO USER** when:

   - **Complex Breaking Changes**: Framework changes conflict fundamentally with existing project structure
   - **Obsolete Documents**: Framework no longer includes documents that contain critical project information
   - **Major Version Jump**: Multiple version changes that require sequential migration
   - **Content Conflicts**: New framework requirements incompatible with existing content
   - **Custom Modifications**: Project has custom additions that don't align with framework updates

2. **New Documents Handling**:

   - **Detect**: Framework requires documents that don't exist in current project
   - **Strategy**: Create new documents using framework templates
   - **Content Population**:
     - Extract relevant content from existing documents
     - Leave TODO placeholders for content that must be created by project team
     - Document what information needs to be gathered from stakeholders

3. **Obsolete Documents Handling**:

   - **Detect**: Framework no longer includes documents that exist in project
   - **Content Preservation Strategy**:
     - Extract all valuable content before deletion
     - Map content to appropriate locations in current framework documents
     - Archive original documents with clear naming (e.g., `ARCHIVED-document-name.md`)
     - Create migration log documenting what content moved where

4. **Version Jump Management**:

   - **Multiple Version Updates**: Break down into sequential migrations
   - **Incremental Validation**: Validate framework compliance after each version step
   - **Checkpoint Strategy**: Create backups before each major migration step

5. **Conflict Resolution Process**:

   - **Content Conflicts**: When existing content doesn't fit new framework structure
   - **Resolution Approaches**:
     - Adapt content to fit new requirements while preserving meaning
     - Restructure content organization to match framework expectations
     - Flag conflicts that require project team input for resolution

### Step 4: Migration Strategy & Risk Assessment

**Objective**: Plan systematic migration for standard cases without losing any critical information

1. **Context-Informed Content Inventory & Classification**:

   **A. Content Audit with Implementation Level Awareness**:

   - Read through each existing document in `.handbook/`
   - **CONTENT AUDIT**: For each section/paragraph, determine correct document per latest framework guidelines
   - **IMPLEMENTATION LEVEL FILTERING**: Only migrate content appropriate for current project's implementation level
   - Classify content as: Stays in same document / Moves to different document / No longer needed / Needs updating / Above current implementation level
   - **MISPLACED CONTENT DETECTION**: Identify content currently in wrong document according to new framework structure
   - **CROSS-DOCUMENT CONTENT MAPPING**: Note content that should be relocated between documents
   - Identify any non-framework files that contain valuable content needing preservation

   **B. Content Maturity-Based Handling**:

   - **Complete Content**: Migrate with full preservation and enhancement
   - **Partial Content**: Migrate existing content, maintain TODO structure for incomplete sections
   - **Placeholder Content**: Update placeholders to match new framework format
   - **Custom Content**: Preserve customizations while ensuring framework compliance

   **C. Usage-Informed Content Prioritization**:

   - **Active Documents**: Prioritize migration to minimize workflow disruption
   - **Referenced Documents**: Ensure cross-references remain functional after migration
   - **Dormant Documents**: Migrate structure but don't over-invest in unused content
   - **Tool-Integrated Content**: Preserve external integrations and automations

2. **Migration Sequence & Dependency Chain Planning**:

   - Determine framework-specified document creation order (typically: business-context → domain-expertise → product-definition → experience-design → functional-requirements → technical-architecture → quality-validation)
   - **MAP DEPENDENCY CHAINS**: Document which documents depend on each document being updated
   - Plan which documents to migrate first based on dependencies
   - **IDENTIFY CASCADE REQUIREMENTS**: For each document change, list all downstream documents that may need updates
   - Create validation checklist for dependency chain verification
   - Identify content that needs to move between documents during update

3. **Risk Mitigation Planning**:
   - Identify any potential information loss scenarios
   - Plan for breaking changes in document structure
   - Determine which existing content might not fit new framework structure
   - Create backup strategy for preserving current state

### Step 5: Document-by-Document Migration

**Objective**: Update each document systematically while preserving all valuable content

**CRITICAL PRINCIPLE**: Create new framework-compliant documents, don't edit existing ones

1. **For Each Document in Dependency Order**:

   - Create new document following latest framework template structure
   - **CONTENT RELOCATION**: Move content to correct document per framework guidelines
   - Migrate all relevant content from existing document (content that belongs in this document)
   - **RECEIVE RELOCATED CONTENT**: Add content moved from other documents that now belongs here
   - **DISTRIBUTE MISPLACED CONTENT**: Move content currently here that belongs in other documents
   - Add any new sections required by framework updates
   - Ensure document headers/metadata match latest framework standards

2. **Cross-Document Validation & Cascade Effect**:
   - Verify each document references correct information from its dependencies
   - **CRITICAL**: When a document changes, validate ALL downstream documents that depend on it
   - Update content in dependent documents that relies on changed upstream information
   - Check for cascade effects: business-context → domain-expertise → product-definition → experience-design → functional-requirements → technical-architecture → quality-validation
   - Maintain data consistency across the entire `.handbook/` structure
   - Ensure no content duplication between documents

### Step 6: Post-Migration Validation & Success Confirmation

**Objective**: Ensure migration is complete, correct, and framework-compliant

1. **Framework Compliance Verification**:

   - Compare each new document against latest framework template
   - Verify all mandatory sections are present and correctly formatted
   - Check document headers match framework requirements
   - Confirm file naming and location conventions are followed

2. **Content Integrity & Dependency Chain Verification**:

   - Ensure no critical information was lost during migration
   - Verify all cross-references between documents are correct and updated
   - **CASCADE VALIDATION**: For each modified document, verify ALL dependent documents still reference correct information
   - Check dependency chain integrity: If business-context changed → validate domain-expertise → validate product-definition → etc.
   - Confirm that changes in upstream documents are properly reflected in downstream documents
   - **CONTENT PLACEMENT VALIDATION**: Verify all content is in the correct document per framework guidelines
   - **NO ORPHANED CONTENT**: Ensure no content was left in wrong documents or lost during relocation
   - Check that content is properly categorized per framework guidelines
   - Confirm no important business context, technical decisions, or requirements were dropped

3. **Project Integration & Final Validation**:

   - Update `CLAUDE.md` to reference new framework version
   - Test that documentation structure supports development workflow
   - Ensure all stakeholders can find information in expected locations
   - Validate that migrated documents still serve their intended purpose for the project team

4. **Migration Success Verification**:

   **BEFORE CLEANUP** - Verify these critical checkpoints:

   ✅ **Framework Compliance**: Every document matches latest framework template structure  
   ✅ **Content Preservation**: All critical business information preserved (no data loss)  
   ✅ **Content Organization**: All content located in correct document per framework guidelines  
   ✅ **Cross-References**: All document dependencies and references work correctly  
   ✅ **Version Consistency**: `CLAUDE.md` and document headers reflect correct framework version  
   ✅ **Dependency Chain**: Upstream/downstream document relationships intact  
   ✅ **Project Usability**: Team can effectively use updated documentation structure

   **IF ANY CHECKPOINT FAILS**: Do not proceed with cleanup - escalate to user for manual review

5. **Rollback Strategy**:

   **Before migration**: Document current state and create recovery plan

   **If migration fails**:

   - Preserve all generated content in `MIGRATION-ATTEMPT-[date]/` directory
   - Document specific failures and conflicts encountered
   - Provide clear rollback instructions
   - Escalate to user with detailed analysis of why migration couldn't complete

## Migration Type Quick Reference

### Expected Outcomes by Migration Type

**No Action** (Version already current / No meaningful changes):

- Simple confirmation message
- No file changes
- Update any outdated version references

**Light Update** (Minor formatting/metadata changes):

- Headers/metadata updates
- Minor formatting adjustments
- No structural changes
- Duration: 5-10 minutes

**Standard Migration** (Typical framework updates):

- Content relocation between documents
- New sections added
- Dependency updates
- Complete migration following all 6 steps
- Duration: 30-60 minutes

**Complex Migration** (Breaking changes/major updates):

- Multiple version jumps handled sequentially
- New documents created
- Obsolete documents archived
- Significant content restructuring
- Duration: 1-3 hours

**Manual Escalation** (Beyond automated capability):

- Clear documentation of what cannot be automated
- Preservation of all existing content
- Detailed analysis of conflicts
- Specific recommendations for manual resolution
- Hand-off to user with clear next steps

## Process Guidelines

### Context-Driven Decision Framework

**When to Ask User**:

- Uncertain about framework requirements or interpretation
- Potential loss of critical business information
- Major structural changes affecting project workflow
- Content doesn't clearly fit new framework structure
- **Implementation level mismatch**: Framework changes suggest different level than current project
- **Usage pattern conflicts**: Changes would disrupt established workflows
- **Custom modifications conflict**: Project customizations incompatible with framework updates

**When to Proceed Autonomously**:

- Clear framework compliance issues (headers, metadata, formatting)
- Content relocation per framework guidelines that matches current implementation level
- Adding new sections required by framework (but appropriate for project level)
- Cross-reference updates between documents
- **Content maturity matches**: Migration preserves existing completion level
- **Usage patterns maintained**: Changes don't disrupt active workflows

### Implementation Level-Specific Guidelines

**Basic Level Projects**:

- Focus only on core framework documents
- Avoid adding advanced sections unless explicitly present in current implementation
- Maintain simple, streamlined approach
- Preserve basic project structure and workflow

**Standard Level Projects**:

- Include all standard framework documents and sections
- Balance completeness with practicality
- Ensure professional project presentation
- Maintain comprehensive but manageable documentation

**Advanced Level Projects**:

- Include all framework features and enterprise sections
- Maintain high level of detail and completeness
- Preserve compliance and regulatory considerations
- Ensure scalable and maintainable documentation structure

### Information Sources (Use in Order)

1. **Framework Repository**: Access https://github.com/adrian-d-hidalgo/clarity-framework directly
2. **CHANGELOG.md**: Primary source for understanding changes between versions
3. **Templates Directory**: Latest structure and format requirements
4. **Current Project**: `.handbook/` directory and `CLAUDE.md` for existing implementation

### Quality Assurance

**For Each Step**:

- Document what you're doing and why (framework compliance rationale)
- List specific changes being made to each document
- **DEPENDENCY IMPACT**: Identify which downstream documents may be affected by changes
- **CASCADE CHECK**: Verify that dependent documents still work correctly after upstream changes
- Identify any risks or potential information loss
- Explain how changes improve framework compliance
- Confirm next steps in migration process

**For Overall Migration**:

- Verify no business-critical information was lost
- Ensure all documents work together as coherent system
- Confirm project team can still effectively use documentation
- Validate framework compliance across entire `.handbook/` structure

## Success Criteria

✅ **Framework Compliance**: All documents match latest framework templates and requirements  
✅ **Content Preservation**: No critical project information lost during migration  
✅ **Content Placement**: All content is located in correct document per framework guidelines  
✅ **Structural Integrity**: Document dependencies and cross-references work correctly  
✅ **Project Usability**: Updated documentation effectively supports project development  
✅ **Version Tracking**: `CLAUDE.md` and document headers reflect correct framework version  
✅ **Clean Implementation**: `.handbook/` structure is organized and framework-compliant

## Migration Philosophy

**Framework First**: When in doubt, prioritize framework compliance while preserving project value  
**Content Safety**: Never delete content without confirming it's obsolete or relocated  
**Content Classification**: Ensure every piece of content is in the document where framework expects it  
**Systematic Approach**: Follow dependency order to avoid breaking cross-document references  
**Cascade Awareness**: Always check downstream impacts when upstream documents change  
**Stakeholder Focus**: Ensure updated documentation serves project team's development needs

## Document Dependency Chain

```
business-context.md
├── → domain-expertise.md
├── → product-definition.md
│   └── → experience-design.md
│       └── → functional-requirements.md
│           └── → technical-architecture.md
│               └── → quality-validation.md
└── → (affects ALL documents - foundational changes require full validation)
```

**Key Dependencies to Monitor**:

- **business-context changes** → Validate ALL downstream documents
- **domain-expertise changes** → Validate product-definition, experience-design, functional-requirements, technical-architecture
- **product-definition changes** → Validate experience-design, functional-requirements
- **experience-design changes** → Validate functional-requirements, technical-architecture
- **functional-requirements changes** → Validate technical-architecture, quality-validation
- **technical-architecture changes** → Validate quality-validation
