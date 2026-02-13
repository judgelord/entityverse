# entityverse

Status: 
🟩 = working 
🟦 = near working
🟨 = in development 

Eventually, this will be an R package to load a suite of packages that detect names and aliases of organized entities. The initial scope of tools focuses on legal entities that may be active in U.S. policymaking or civic life, including: 

- U.S. Legislators: https://judgelord.github.io/legislators/ 🟩
    - Data sources: voteview.com, others
    - IDs linked: ICPSR, [congress.gov bioguide](https://bioguide.congress.gov)
- State legislators 
    - Data sources: 
    - IDs linked: 
- U.S. federal agencies 🟦 https://github.com/judgelord/agencies
    - Data sources: regulations.gov, the federal budget, others
    - IDs linked: unique nested acronyms in the form "DOI_BLM" or "EPA_OAR" or "EOP_OMB_FPPO"
- U.S. State government agencies 
    - Data sources: 
    - IDs linked: 
- U.S. Counties 
    - Data sources: 
    - IDs linked:
- U.S. local governments 
    - Data sources: 
    - IDs linked:
- U.S. corporations: 🟦 https://github.com/judgelord/corporations
    - Data sources: Compustat, CIK 
    - IDs linked:
- U.S. industry associations 
    - Data sources: 990s
    - IDs linked: EIN
- U.S. labor unions
    - Data sources: 990s
    - IDs linked: EIN
- U.S. nonprofits (excluding industry associations and unions)
    - Data sources: 990s
    - IDs linked: EIN
- U.S. campaign donors 🟨 https://github.com/judgelord/donors
    - Data sources: OpenSecrets/CRP 
    - IDs linked: ID, parentID
- U.S. lobbiests 
    - Data sources: 
    - IDs linked:
- Native American Tribes and groups 🟨 
    - Data sources: 
    - IDs linked: (we'll need to make up an ID) 

All will rely on a base tool, [`regextable`](https://judgelord.github.io/regextable/), that uses regular expressions in a lookup table to efficiently search text and link strings matching entities to unique IDs. 
