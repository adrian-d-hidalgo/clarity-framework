# 👥 CLARITY Framework Collaboration Guide

## Roles, Responsibilities and Team Coordination

---

## 🎯 **Framework Overview for Teams**

The **CLARITY Framework** is designed for collaborative product specification creation that enables **successful delegation** to development teams or AI systems. This guide defines how different roles collaborate to create complete, coherent specifications.

### **Core Collaboration Principles**

```yaml
successful_collaboration:
  - Clear ownership per document with cross-functional input
  - Iterative validation between roles at each phase
  - Consistent terminology and cross-references
  - Documentation that serves development, not just process

delegation_success:
  - Each role contributes their domain expertise
  - All roles validate final specifications
  - Clear handoff criteria and success metrics
  - Development team can start without additional questions
```

---

## 👥 **Role Definitions**

### **🎯 Product Manager**

```yaml
primary_responsibility: "Product strategy and business requirements"
primary_ownership:
  [
    "business-context",
    "product-definition",
    "functional-requirements",
    "quality-validation",
  ]
key_skills: ["business_analysis", "user_research", "requirement_gathering"]
deliverables_location: ".handbook/product/"
```

**Core Responsibilities:**

- Define business context and competitive landscape
- Specify product features and user requirements
- Document functional requirements and business logic
- Establish quality validation criteria and acceptance tests
- Coordinate between business stakeholders and technical teams

### **🎨 UX Designer**

```yaml
primary_responsibility: "User experience and interface design"
primary_ownership: ["experience-design"]
key_skills:
  ["user_research", "interaction_design", "visual_design", "prototyping"]
deliverables_location: ".handbook/design/"
```

**Core Responsibilities:**

- Design complete user experience flows
- Create wireframes and interactive prototypes
- Develop design systems and visual specifications
- Ensure accessibility and usability standards
- Collaborate with PM on user requirements and with architects on technical feasibility

### **🏗️ Software Architect**

```yaml
primary_responsibility: "Technical architecture and system design"
primary_ownership: ["architecture"]
key_skills: ["system_design", "technology_selection", "scalability_planning"]
deliverables_location: ".handbook/technical/"
```

**Core Responsibilities:**

- Design scalable technical architecture
- Select appropriate technology stack
- Define system integration patterns
- Create technical documentation and diagrams
- Establish development standards and practices
- Document architecture decisions (ADRs)

### **🧪 QA Lead**

```yaml
primary_responsibility: "Quality assurance and testing implementation"
primary_ownership: ["qa-deliverables"]
collaborative_ownership: ["quality-validation"]
key_skills:
  ["test_planning", "test_automation", "quality_processes", "test_execution"]
deliverables_location: ".handbook/quality/"
```

**Core Responsibilities:**

- Create comprehensive testing strategy and implementation plan
- Develop detailed test matrices and test cases
- Design test environments and data management strategy
- Implement test automation frameworks
- Execute testing phases and track quality metrics
- Collaborate with PM on overall quality validation strategy
- Review all documents for testability and quality criteria

### **🏢 Business Stakeholder**

```yaml
primary_ownership: ["Strategic input and validation"]
core_responsibilities:
  - Provide business strategy and market context
  - Validate business requirements and priorities
  - Approve scope and resource allocation
  - Review and sign off on final specifications

collaboration_points:
  - Input to business context and product definition
  - Validation at key checkpoints throughout process
  - Final approval for development handoff
  - Change management and stakeholder communication

skills_required:
  - Business strategy and market understanding
  - Stakeholder management
  - Change management
  - Resource planning and budget oversight
```

### **💻 Development Team Lead**

```yaml
primary_ownership: ["Technical feasibility validation"]
core_responsibilities:
  - Validate technical feasibility throughout process
  - Provide implementation estimates and constraints
  - Review specifications for development readiness
  - Confirm handoff readiness and success criteria

collaboration_points:
  - Reviews technical architecture for implementability
  - Validates functional specifications for clarity
  - Provides input on technology choices and constraints
  - Final validation before development starts

skills_required:
  - Development team leadership
  - Technical implementation expertise
  - Estimation and planning
  - Code quality and development practices
```

---

## 📋 **Responsibility Matrix**

| **Document**                | **Primary Owner**  | **Key Collaborators**               | **Reviewers**               | **Final Approver**   |
| --------------------------- | ------------------ | ----------------------------------- | --------------------------- | -------------------- |
| **business-context**        | Product Manager    | Business Stakeholder                | All roles                   | Business Stakeholder |
| **domain-expertise**        | Product Manager    | Domain Expert                       | All roles                   | Product Manager      |
| **product-definition**      | Product Manager    | UX Designer, QA Lead                | All roles                   | Product Manager      |
| **experience-design**       | UX Designer        | Product Manager                     | Software Architect, QA Lead | UX Designer          |
| **functional-requirements** | Product Manager    | Software Architect, UX Designer     | Development Lead, QA Lead   | Product Manager      |
| **architecture**            | Software Architect | Development Lead                    | All technical roles         | Software Architect   |
| **quality-validation**      | Product Manager    | QA Lead, All roles                  | Development Lead            | Product Manager      |
| **qa-deliverables**         | QA Lead            | Product Manager, Software Architect | Development Lead            | QA Lead              |

### **Cross-Document Validation**

```yaml
coherence_validation:
  - All roles review for terminology consistency
  - Dependencies between documents verified by owners
  - Cross-references validated by contributing roles
  - Final coherence check by QA Lead

integration_checkpoints:
  - After business context: All roles align on priorities
  - After product definition: UX and Architecture validate scope
  - After experience design: Architecture and QA validate feasibility
  - After functional specs: Development validates implementability
  - After technical architecture: All roles validate completeness
  - Final review: All roles sign off on delegation readiness
```

---

## 🔄 **Collaboration Workflow**

### **Phase 1: Discovery (25% effort)**

#### **Week 1: Business Foundation**

```yaml
business_context_creation:
  lead: "Product Manager"
  day_1-2:
    activities: "Stakeholder interviews, competitive analysis"
    collaborators: "Business Stakeholder, UX Designer (user research)"
    output: "Draft business context"

  day_3-4:
    activities: "Business context review and validation"
    collaborators: "All roles review for technical feasibility"
    output: "Validated business priorities and constraints"

  day_5:
    activities: "Business context finalization"
    approval: "Business Stakeholder sign-off"
    handoff: "Context available for product definition"

product_definition_creation:
  lead: "Product Manager"
  day_1-2:
    activities: "Feature prioritization, user story creation"
    collaborators: "UX Designer, QA Lead (acceptance criteria)"
    output: "Draft product definition"

  day_3-4:
    activities: "Scope validation and feasibility check"
    collaborators: "Software Architect, Development Lead"
    output: "Validated feature set and scope boundaries"

  day_5:
    activities: "Product definition finalization"
    approval: "Product Manager sign-off"
    handoff: "Scope ready for design phase"
```
