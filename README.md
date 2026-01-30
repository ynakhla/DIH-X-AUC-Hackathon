# Deloitte x AUC Hackathon

## Introduction

Welcome to the Deloitte x AUC Hackathon. As potential future consultants at Deloitte, you will face a reality that defines the consulting profession: clients come to us with problems, not solutions.

### The Consultant's Challenge

Clients expect consultants to diagnose their challenges and architect innovative solutions. You will not receive a step-by-step guide, just like in the real world. Success requires both technical excellence and business acumen across four key dimensions:

**Technical Skills**: Can you build your solution?

**Business Thinking**: Should you build it? What value does it provide?

**Team Work**: Can you deliver it together?

**Communication**: Can you sell your solution?

### How to Approach This Challenge

Each use case below presents a client with a real business problem. The business questions provided are meant to help guide your thinking and give you ideas on possible features to implement. Your approach should be:

1. Frame the business problem and understand the value proposition
2. Identify which business questions your solution will address
3. Design and implement technical features that deliver measurable business impact
4. Document how your solution creates value for the client

Remember: clients look for measurable impact, scalability, and competitive advantages. Think like a consultant, build like an engineer.

---

## Data Processing & Optimization

### Large File Handling

To ensure optimal performance and manageability of the dataset, we have processed large data files:

**Menu Engineering - Payment Data Split**
- **Original File**: `fct_payments.csv` (2.16 GB, ~76.7 million records)
- **Processed Files**:
  - `fct_payments_part1.csv` (1.03 GB, ~38.4 million records including header)
  - `fct_payments_part2.csv` (1.13 GB, ~38.4 million records including header)

**Rationale**: The original payment transaction file exceeded GitHub's recommended file size limits and was too large for efficient processing. By splitting it into two manageable parts, we enable:
- Faster data loading and processing
- Better version control with Git LFS
- Parallel processing capabilities for analytics
- Reduced memory requirements for data analysis

**Git LFS Configuration**: All CSV files are tracked using Git Large File Storage (LFS) to maintain repository performance while preserving full dataset access.

---

## Repository & Documentation Requirements

### Required Components

**README.md File**
- Must be present at the root of your repository
- Should include a clear project description and the problem it solves
- List all features and functionalities
- Document all technologies, frameworks, and external APIs used
- Provide step-by-step installation instructions
- Include usage guidelines and examples
- List all team members with their roles and contributions

**Code Organization**
- Use proper file extensions for all code files
- Maintain a clear and logical folder structure
- Separate concerns into appropriate directories (models, services, utils, api)
- Include an entry point file (e.g., main.py, index.js)

**Dependencies Management**
- Include a dependencies file (requirements.txt for Python, package.json for Node.js, etc.)
- List all libraries and frameworks required to run the project
- Specify version numbers where applicable

**Code Quality**
- Add meaningful comments and docstrings to all functions and classes
- Include file headers explaining the purpose of each module
- Follow language-specific best practices and conventions
- Ensure code runs without errors

**Security**
- Do not include sensitive data such as API keys, passwords, or tokens
- Use environment variables for configuration
- Include a .gitignore file to exclude sensitive or unnecessary files

**Testing**
- Include test files in a dedicated tests directory
- Document how to run tests

**Additional Documentation**
- Provide architecture overview or diagrams (optional but recommended)
- Include any additional documentation in a docs directory

### Repository Access
- Repository must be public
- Use the main branch for submission
- Ensure all team members have appropriate access


---

## Use Cases (Clients)

### Fresh Flow Markets: Inventory Management

**The Challenge**

Restaurant and grocery owners face a relentless balancing act. Over-stocking leads to waste and expired inventory eating away at profits. Under-stocking causes stockouts, lost revenue, and frustrated customers. The root cause? Poor demand forecasting. Without accurate predictions, businesses are trapped in a cycle of unnecessary costs, reduced profitability, and unsustainable operations. FreshFlow needs intelligent systems, not gut instinct.

**Potential Business Questions**

The following questions are provided to help guide your thinking and inspire potential features for your solution:

- How do we accurately predict daily, weekly, and monthly demand?
- What prep quantities should kitchens prepare to minimize waste?
- How can we prioritize inventory based on expiration dates?
- What promotions or bundles can move near-expired items profitably?
- How do external factors (weather, holidays, weekends) impact sales?

---

### Flavor Flow Craft: Menu Engineering

**The Challenge**

FlavorCraft sits on a goldmine of historical sales data—every order, every customer preference—yet they're making menu decisions on hunches. They don't know which dishes are secretly losing money, or what tweaks could turn underperformers into bestsellers. This isn't just a missed opportunity; it's revenue left on the table. Your mission is to create a data-driven assistant that analyzes their menu and sales data, suggesting improvements to items, descriptions, and pricing. But don't stop there—your client manager encourages innovative thinking beyond the obvious.

**Potential Business Questions**

The following questions are provided to help guide your thinking and inspire potential features for your solution:

- Which menu items are stars, plowhorses, puzzles, or dogs?
- How should we adjust pricing to maximize profitability?
- What wording or descriptions increase item sales?
- Which items should be promoted, re-engineered, or eliminated?
- What hidden patterns exist in customer purchasing behavior?



### Quick Serve Kitchens: Shift Planning

**The Challenge**

Monday's schedule looks perfect. Wednesday: three call-offs. Friday: foot traffic doubles because TikTok made your item viral. The schedule is now a dumpster fire. This is QuickServe's weekly reality. The core problem? Accurately predicting and meeting wildly fluctuating customer demand to ensure optimal staffing on every shift. Too few people means terrible service and burnout. Too many means spiraling labor costs. QuickServe needs a Shift Wizard—an intelligent system that monitors schedules, coverage, PTO, surprise events, and constantly recommends the next best move.

**Potential Business Questions**

The following questions are provided to help guide your thinking and inspire potential features for your solution:

- How do we predict demand spikes from social media, weather, or events?
- What's the optimal staffing level for each shift?
- How do we quickly adjust when call-offs happen?
- How can we balance labor costs with service quality?
- How do we incorporate employee preferences while meeting business needs?

---

## Evaluation Criteria

### Documentation Quality
Your project documentation will be evaluated based on the clarity and completeness of your README file, the presence of code comments and docstrings, and the overall organization of documentation materials.

### Code Architecture & Modularity
The structure and organization of your codebase will be assessed, including proper separation of concerns, logical folder hierarchy, and modular design patterns that promote maintainability and scalability.

### Team Collaboration
Collaboration will be evaluated through GitHub commit history, ensuring all team members have contributed meaningfully to the project with clear and descriptive commit messages.

### AI/ML Integration
If your solution incorporates artificial intelligence or machine learning components, the implementation, documentation, and effectiveness of these technologies will be evaluated.

### Business Value & Innovation
Your solution will be assessed on its practical applicability, innovation in addressing the problem statement, and potential real-world impact for the specified use case.

### Technical Implementation
The technical execution of your solution will be reviewed, including code quality, proper use of technologies and frameworks, error handling, and overall functionality.