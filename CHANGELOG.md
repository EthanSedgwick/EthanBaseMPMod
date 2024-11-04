
# Change Log
All notable changes to this project will be documented in this file.
 
The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).


## [0.1] - yyyy-mm-dd

### Added
- Added Ethan Leaders
  - Takes the PUIR approach of splitting attack and defense into separate columns, and adding colours to good leaders while retaining Vanilla leader distribution
 
### Changed
- Navy changes
  - Defines
    - NAVAL_COMBAT_STACKING_TARGET_CHANGE: 0.03 -> 0.1 :chart_with_upwards_trend:
    - NAVAL_COMBAT_STACKING_TARGET_SELECT: 0.2 -> 0.3 :chart_with_upwards_trend:
    - NAVAL_COMBAT_MAX_TARGETS: 6 -> 4 :chart_with_downwards_trend:
    <br /><sup>Makes larger navies of low quality less effective against smaller navies of lower quality. Incentivises high tier ships.</sup>

  
- Gas changes
  Defines: GAS_ATTACK_MODIFIER: 3 -> 1
  Invention: 
  <br /><sup>Reintroduces randomness to Gas and Gas defense by nerfing its overall impact, allowing Gas to be relevant again.</sup>

- War
  - TWS_CB_LIMIT_DEFAULT: 100 -> 75 :chart_with_downwards_trend:
  <br /><sup>Makes it so players cannot win wars just off ticking war score, you must also be winning via other factors by atleast 25%.</sup>
  - MOBILIZATION_SPEED_RAILS_MULT: 3.0 -> 3.5 :chart_with_upwards_trend: -- 
  <br /><sup>Small buff to high tech nations / Railroads</sup>

- Diplomacy
  - Diplo points
    - Set to 0 :x:
      - ADDWARGOAL_DIPLOMATIC_COST
      - PEACE_DIPLOMATIC_COST
      - ALLIANCE_DIPLOMATIC_COST
      - CANCELALLIANCE_DIPLOMATIC_COST
      - ASKMILACCESS_DIPLOMATIC_COST
      - CANCELASKMILACCESS_DIPLOMATIC_COST
      - GIVEMILACCESS_DIPLOMATIC_COST
      - CANCELGIVEMILACCESS_DIPLOMATIC_COST
    - BASE_MONTHLY_DIPLOPOINTS: 0.3 -> 1.5 :chart_with_upwards_trend:
    <br /><sup>Removes diplo point cost for majority of actions and all player to player interactions, but keeps diplo point cost for actions related to influencing nations</sup>
  - MAKE_CB_RELATION_LIMIT: 100 -> 120 :chart_with_upwards_trend:
  - LARGE_POPULATION_INFLUENCE_PENALTY: -0.4 -> -0.25 :chart_with_downwards_trend:
  <br /><sup>Allows large nations like the Ottomans to still be influenced, even when they scale</sup>

- Economy
  - RGO_SUPPLY_DEMAND_FACTOR_FIRE: **0.4 -> 0.02** :chart_with_downwards_trend: 
  <br /><sup>Gives the user more breathing room to save or maintain their planned economy after electing a liberal party</sup>
  - MIN_NUM_FACTORIES_PER_STATE_BEFORE_DELETING_LASSIEZ_FAIRE: **2 > 9** :x: 
  <br /><sup>Gives the user more breathing room to save or maintain their planned economy after electing a liberal party</sup>
  - FACTORY_UPGRADE_EMPLOYEE_FACTOR: **0.8 -> 0.75** :chart_with_downwards_trend: 
  <br /><sup>Convenience change</sup>
  - CAPITALIST_BUILD_FACTORY_STATE_EMPLOYMENT_PERCENT: **0.7 > 1.1** :x: 
  <br /><sup>Changes aimed to prevent Capitalists from creating new factories</sup>
  - NONCORE_TAX_PENALTY: **-0.05 -> -0.10** :chart_with_upwards_trend:
  - BASE_COUNTRY_TAX_EFFICIENCY: **0.2 -> 0.22** :chart_with_upwards_trend:



- Misc
  - AI Army Changes
  - AI_CAVALRY_PROPORTION -   **0.15 > 0.1**  :chart_with_downwards_trend:
  - AI_SUPPORT_PROPORTION -   **0.3 -> 0.5**  :chart_with_downwards_trend:
  - AI_SPECIAL_PROPORTION -   **0.15 -> 0**   :chart_with_downwards_trend:
  <br /><sup>Makes the AI build Reno meta stacks, so they are less like paper tigers.</sup>
  - REDUCTION_AFTER_DEFEAT -  **3.0 > 4.0**   :chart_with_upwards_trend: 
  <br /><sup>After a rebellion is being defeated in combat, its pop militancy will be divided by this number.</sup>
  - PEACE_BASE_RELUCTANCE -   **20 -> 15**    :chart_with_downwards_trend: 
  <br /><sup>AI base stubbornness to refuse peace.</sup>
  - Disabled Newspapers
  - Disabled Crises
