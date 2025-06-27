# 🏢 Business Context

## Foundation for Technical Decisions

**Document:** business-context  
**Framework:** CLARITY Framework v1.0
**Version:** 1.0  
**Date:** [YYYY-MM-DD]  
**Security Level:** [Standard/Elevated/Critical]

---

## ⚡ **COMPLETION GUIDE**

### **🎯 CORE Sections (Complete First - Essential):**

1. **Business Model and Value Proposition** - Affects revenue architecture, pricing logic ⏱️ _30-45 min_
2. **User Types and Market Context** - Affects UX decisions, performance requirements ⏱️ _45-60 min_
3. **Security Requirements** - Affects technical architecture, compliance features ⏱️ _15-30 min_
4. **Success Metrics and Priorities** - Affects monitoring, analytics, performance optimization ⏱️ _30-45 min_

**Total CORE time: 2-3 hours**

### **📈 EXTENDED Sections (Complete When Time Allows):**

1. **Detailed Competitive Analysis** - Affects feature prioritization, differentiation
2. **Comprehensive Constraint Documentation** - Affects technology choices, timelines
3. **Long-term Vision and Roadmap** - Affects scalability decisions, technical debt planning

---

## 🎯 **Document Purpose**

This document establishes the **minimum business context** necessary for making correct technical decisions during product development. It focuses exclusively on information that directly affects how the product should be built, not general market analysis.

> **Principle:** Only include business information that influences technical implementation decisions.

---

## ⚖️ **Decision Frameworks**

### **Trade-off Decision Matrix**

When business and technical requirements conflict, use this priority framework:

**Performance vs Features:**

- **Choose Performance when:** User experience is critical, high-scale requirements, real-time needs
- **Choose Features when:** MVP validation, competitive pressure, limited technical resources
- **Decision criteria:** User impact > business impact > technical complexity

**Quality vs Speed:**

- **Choose Quality when:** Security critical, regulated industry, long-term product
- **Choose Speed when:** Market window closing, proof of concept, competitive response
- **Decision criteria:** Risk assessment > business timeline > technical debt tolerance

**Cost vs Capability:**

- **Choose Cost when:** Budget constraints, early stage startup, uncertain market
- **Choose Capability when:** Competitive advantage, proven market, scale requirements
- **Decision criteria:** ROI analysis > strategic importance > implementation complexity

### **Conflict Resolution Process**

1. **Identify the conflict:** [Business requirement] vs [Technical constraint]
2. **Apply decision matrix:** Use framework above
3. **Document the decision:** Record rationale for future reference
4. **Set review trigger:** When to revisit this decision

---

## ✅ **Quality Gates**

**Before proceeding to next documents, ensure:**

- [ ] Security level is clearly defined (affects all technical decisions)
- [ ] Primary user types are documented (affects UX and performance requirements)
- [ ] Success metrics are specified (affects monitoring and analytics requirements)
- [ ] Business model is clear (affects payment processing, pricing features)
- [ ] Trade-off preferences are documented (guides technical decisions)

---

## 📋 **Business Model and Value Proposition**

### **Core Value Proposition**

**Primary Problem Solved:**

- **Problem Description:** [What specific problem does this product solve?]
- **Impact Assessment:** [How significant is this problem for users?]
- **Current Solutions:** [How do users solve this problem today?]

**Unique Value:**

- **Differentiation:** [What makes this solution unique?]
- **Competitive Advantage:** [Why would users choose this over alternatives?]
- **Business Impact:** [What business outcome does this create?]

### **Business Model**

**Monetization:**

- **Revenue Model:** [How does the product generate revenue?]
- **Pricing Strategy:** [What is the pricing approach?]
- **Target Market Size:** [What is the addressable market?]

**Sustainability:**

- **Cost Structure:** [What are the main operational costs?]
- **Scalability Factors:** [What enables/limits business scaling?]
- **Success Metrics:** [How is business success measured?]

---

## 🎭 **User Types and Market Context**

### **Primary User Types**

**User Type 1:**

- **Name:** [e.g., "Busy Professional Mom"]
- **Description:** [e.g., "Working mothers, 30-45 years old, managing career and family"]
- **Primary Needs:** [e.g., "Quick, reliable solutions that save time and reduce stress"]
- **Technical Context:** [e.g., "Comfortable with mobile apps, prefers simple interfaces"]
- **Usage Patterns:** [e.g., "Quick sessions during commute, evening planning"]

**User Type 2:**

- **Name:** [e.g., "Small Business Owner"]
- **Description:** [e.g., "Entrepreneurs running 1-10 person businesses"]
- **Primary Needs:** [e.g., "Cost-effective tools that improve efficiency and revenue"]
- **Technical Context:** [e.g., "Moderate technical skills, values integrations with existing tools"]
- **Usage Patterns:** [e.g., "Daily use during business hours, mobile + desktop"]

_Add additional user types as needed_

### **Market Position**

```yaml
competitive_landscape:
  direct_competitors:
    - name: "[Competitor name]"
      strength: "[Their main advantage]"
      weakness: "[Where they fall short]"
      technical_approach: "[How they solve the problem technically]"

  indirect_competitors:
    - category: "[Alternative solution type]"
      examples: "[Specific examples]"
      why_chosen: "[Why users might choose this instead]"

positioning_strategy:
  target_segment: "[Which market segment to focus on]"
  positioning_message: "[How to position against competition]"
  technical_implications: "[How positioning affects technical decisions]"
```

---

## 🔒 **Compliance and Security Requirements**

### **Security Level: [Standard/Elevated/Critical]**

#### **Standard Security Requirements**

```yaml
# For basic web/mobile applications
basic_compliance:
  - GDPR basic compliance (consent, data rights)
  - Standard authentication and authorization
  - HTTPS mandatory for all communications
  - Basic input validation and XSS protection

technical_implications:
  - JWT/OAuth authentication sufficient
  - Basic audit logging for user actions
  - Standard password policies
  - Basic encryption for sensitive data at rest
```

#### **Elevated Security Requirements** (if applicable)

```yaml
# For B2B, sensitive data, basic healthcare
enhanced_compliance:
  - SOC 2 Type II compliance requirements
  - Data residency and sovereignty requirements
  - Role-based access control (RBAC)
  - Audit logging for all system actions

technical_implications:
  - Multi-factor authentication (MFA) required
  - Enhanced encryption standards
  - Detailed audit trails
  - Data backup and recovery procedures
```

#### **Critical Security Requirements** (if applicable)

```yaml
# For fintech, regulated healthcare, government
strict_compliance:
  - Industry-specific regulations (HIPAA, PCI-DSS, SOX)
  - Zero-trust security architecture
  - Complete data governance and lineage
  - Regular security audits and certifications

technical_implications:
  - End-to-end encryption requirements
  - Advanced threat detection and monitoring
  - Comprehensive compliance reporting
  - Disaster recovery and business continuity
```

---

## 📊 **Success Metrics and Priorities**

### **Business Success Metrics**

```yaml
primary_kpis:
  metric_1:
    name: "[Metric name]"
    definition: "[How is it measured?]"
    target: "[What is the goal?]"
    technical_impact: "[How does this affect technical decisions?]"

  metric_2:
    name: "[Metric name]"
    definition: "[How is it measured?]"
    target: "[What is the goal?]"
    technical_impact: "[How does this affect technical decisions?]"

secondary_metrics:
  - "[Supporting metrics that inform technical trade-offs]"
  - "[Performance metrics that guide technical implementation]"
```

### **Business Priorities**

```yaml
priority_1: "[Most critical business requirement]"
priority_2: "[Second most critical requirement]"
priority_3: "[Third most critical requirement]"

trade_off_guidance:
  performance_vs_features: "[When to prioritize performance over new features]"
  quality_vs_speed: "[When to prioritize quality over delivery speed]"
  cost_vs_capability: "[When to prioritize cost savings over capabilities]"
```

---

## ⚖️ **Constraints and Dependencies**

### **Business Constraints**

```yaml
budget_constraints:
  development_budget: "[Available budget for development]"
  operational_budget: "[Ongoing operational budget limits]"
  cost_per_user_target: "[Target cost per user/transaction]"

timeline_constraints:
  market_window: "[When does the product need to be in market?]"
  funding_milestones: "[Key dates tied to funding/investment]"
  competitive_pressure: "[Timeline pressure from competition]"

resource_constraints:
  team_size_limits: "[Maximum team size available]"
  skill_availability: "[Available technical skills and gaps]"
  vendor_relationships: "[Existing vendor relationships to leverage]"
```

### **Technical Constraints**

```yaml
platform_requirements:
  target_platforms: "[Web, mobile, desktop requirements]"
  device_support: "[Minimum device requirements]"
  browser_support: "[Required browser compatibility]"

integration_requirements:
  existing_systems: "[Systems that must integrate with]"
  data_migration: "[Data that needs to be migrated]"
  api_dependencies: "[External APIs that must be supported]"

performance_requirements:
  response_time: "[Maximum acceptable response times]"
  concurrent_users: "[Expected concurrent user load]"
  data_volume: "[Expected data volume and growth]"
```

---

## 🎯 **Product Vision and Roadmap Context**

### **Product Vision**

```yaml
long_term_vision:
  vision_statement: "[Where should this product be in 2-3 years?]"
  market_expansion: "[How might the market expand?]"
  technical_evolution: "[How should the technology evolve?]"

current_phase:
  phase_description: "[What phase of product development is this?]"
  success_criteria: "[How do we know this phase is successful?]"
  next_phase_preparation: "[What technical decisions support future phases?]"
```

### **Strategic Dependencies**

```yaml
business_dependencies:
  - dependency: "[External business factor]"
    impact: "[How it affects product decisions]"
    mitigation: "[How to reduce dependency risk]"

market_dependencies:
  - dependency: "[Market condition or trend]"
    impact: "[How it affects technical architecture]"
    timeline: "[When this factor becomes critical]"
```

---

## ✅ **Validation Checklist**

### **Completeness Check**

- [ ] Business value proposition clearly defined
- [ ] All user types identified and characterized
- [ ] Competitive position understood and documented
- [ ] Security/compliance requirements identified
- [ ] Success metrics defined with technical implications
- [ ] Constraints and dependencies documented
- [ ] Information directly affects technical decisions

### **Quality Check**

- [ ] All information is specific and actionable
- [ ] No generic industry information without specific impact
- [ ] Security level appropriate for application type
- [ ] Constraints are realistic and verifiable
- [ ] Success metrics are measurable
- [ ] Document serves development needs, not just process

### **Security Integration Check**

- [ ] Security level clearly identified and justified
- [ ] Compliance requirements specific to application domain
- [ ] Technical implications of security requirements documented
- [ ] Risk assessment appropriate for security level

---

## 📝 **Document Metadata**

```yaml
document_info:
  creation_date: "[YYYY-MM-DD]"
  last_updated: "[YYYY-MM-DD]"
  version: "1.0"

stakeholders:
  primary_author: "[Name and role]"
  reviewers: ["[Name and role]", "[Name and role]"]
  approver: "[Name and role]"

dependencies:
  inputs_from: []
  outputs_to: ["product-definition", "experience-design"]

security_classification: "[Standard/Elevated/Critical]"
framework_compliance: "CLARITY Framework v1.0"
```

---

## 🤖 **AI VALIDATION PROMPTS**

**Use these prompts to validate document completeness with AI assistance:**

1. **Completeness Check:** "Review this business context document. Are all CORE sections complete with specific, actionable information? Identify any vague or placeholder content."

2. **Technical Impact Validation:** "Based on this business context, what specific technical decisions will be influenced? Are security level, user types, and success metrics clear enough to guide architecture?"

3. **Trade-off Clarity:** "Are the documented trade-off preferences specific enough to resolve conflicts between performance vs features, quality vs speed, and cost vs capability?"

4. **User Type Specificity:** "Do the user types include enough technical context and usage patterns to inform UX design and performance requirements?"

5. **Success Metrics Validation:** "Are the success metrics measurable and specific enough to implement monitoring and analytics requirements?"

---

**Next Document:** [domain-expertise](02_domain_expertise_template.md) (if required) or [product-definition](03_product_definition_template.md)

> **📁 Implementation Note**: When using this template, create the working file as `.handbook/product/business-context.md` - this is a **PM responsibility**.
