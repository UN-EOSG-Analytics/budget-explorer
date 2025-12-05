Claude analysis of document structure:

UN Budget Document A_80_400 - Structure Analysis

DOCUMENT STRUCTURE:
==================
1. Chapters I-III: Context and proposals (not budget data)
2. Chapter IV: Revised resource requirements (THE KEY DATA)
   - IV.A: Overall summary (Table 5 and 6 - already extracted)
   - IV.B: Details by budget section/entity (59 sections, Tables 21-215)
   - IV.C: Special political missions (37 missions, Tables 216-340)
3. Chapter V: Actions requested (procedural)
4. Annex: Organizational charts

EXTRACTABLE DATA PER ENTITY SECTION (IV.B):
===========================================
Each of the 59 entity sections contains:
1. "Resource changes by object of expenditure" table:
   - Rows: Posts, Other staff costs, Hospitality, Travel, Contractual services, 
           General operating expenses, Supplies, Furniture, etc.
   - Cols: 2025 approved | 2026 proposed | Changes (redeployed) | Changes (other) | 2026 revised

2. "Proposed posts by category and grade" table:
   - Rows: Professional (USG, ASG, D-2, D-1, P-5, P-4, P-3, P-2/1), General Service (PL, OL)
   - Cols: 2025 approved | Proposed changes | 2026 proposed

3. "Proposed post actions" table (when applicable):
   - Lists specific post changes: abolishments, redeployments, reclassifications
   - Cols: Action | Post | Source/Destination

4. Narrative paragraphs explaining:
   - Total budget figure and variance percentages
   - Breakdown by efficiency category:
     * Cost optimization (travel, GTA, contractual services)
     * Functional streamlining (post abolishments, redistribution)
     * Organizational optimization (restructuring)
     * Leveraging technology (IT, virtual meetings)
     * Allocative efficiencies (deliverable adjustments)

EXTRACTABLE DATA FOR SPMs (IV.C):
=================================
37 missions organized by thematic cluster:
- Cluster I: Special/personal envoys (12 missions)
- Cluster II: Sanctions monitoring teams (10 missions)  
- Cluster III: Regional offices/political processes (13 missions)
- Backstopping posts (2)

Each mission has:
1. "Financial resources" table (similar structure to regular budget)
2. "Human resources" table (posts by category/grade)
3. "Changes to human resources" table (specific post actions)
4. Narrative text

RECOMMENDED EXTRACTION APPROACH:
================================
1. For quantitative data:
   - Extract all "resource changes by object of expenditure" tables -> entity-level spending by category
   - Extract all "proposed posts by category and grade" tables -> entity-level staffing
   - Extract "proposed post actions" tables -> individual post changes

2. For qualitative data:
   - Parse narratives to extract:
     * Total budget amounts mentioned
     * Efficiency category breakdowns (amounts per category)
     * Specific measures described

3. Link everything via:
   - Section number (1, 2, 3, ..., 29A, 29B, etc.)
   - Entity name (matching to Table 6)
   - Table numbers (for traceability)

KEY OBSERVATIONS:
=================
- 18 Table 6 entities have no detailed section (legislative bodies, oversight, etc.)
- Document has 59 entity sections but Table 6 only has 46 entities (some sections are sub-entities)
- SPM is treated as a single line in Table 6 but has 37 detailed missions in the document
- Some entities have both regular budget AND support account tables