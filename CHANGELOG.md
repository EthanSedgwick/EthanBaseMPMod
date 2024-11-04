
# Change Log
All notable changes to this project will be documented in this file.
 
The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).


## [0.1] - yyyy-mm-dd
 
Here we write upgrading notes for brands. It's a team effort to make them as
straightforward as possible.
 
### Added
- Added Ethan Leaders
  Takes the PUIR approach of splitting attack and defense into separate columns, and adding colours to good leaders
  Retains Vanilla leader distribution, instead of PUIR custom distribution
- [PROJECTNAME-YYYY](http://tickets.projectname.com/browse/PROJECTNAME-YYYY)
  PATCH Ticket title goes here.
 
### Changed
- Navy changes
  Defines[^1]
    NAVAL_COMBAT_STACKING_TARGET_CHANGE: 0.03 -> 0.1
    NAVAL_COMBAT_STACKING_TARGET_SELECT: 0.2 -> 0.3
    NAVAL_COMBAT_MAX_TARGETS: 6 -> 4 # Ine

  
- Gas changes[^2]
  Defines: GAS_ATTACK_MODIFIER: 3 -> 1
  Invention: 

- War
  TWS_CB_LIMIT_DEFAULT: 100 -> 75[^3]
  MOBILIZATION_SPEED_RAILS_MULT: 3.0 -> 3.5 -- Small buff to high tech nations / Railroads

- Diplomacy
  Diplo points[^4]
    Set to 0
      ADDWARGOAL_DIPLOMATIC_COST
      PEACE_DIPLOMATIC_COST
      ALLIANCE_DIPLOMATIC_COST
      CANCELALLIANCE_DIPLOMATIC_COST
      ASKMILACCESS_DIPLOMATIC_COST
      CANCELASKMILACCESS_DIPLOMATIC_COST
      GIVEMILACCESS_DIPLOMATIC_COST
      CANCELGIVEMILACCESS_DIPLOMATIC_COST
    BASE_MONTHLY_DIPLOPOINTS: 0.3 -> 1.5
  MAKE_CB_RELATION_LIMIT: 100 -> 120
  LARGE_POPULATION_INFLUENCE_PENALTY: -0.4 -> -0.25[^5]

- Economy
  - RGO_SUPPLY_DEMAND_FACTOR_FIRE: **0.4 -> 0.02** <sup>Gives the user more breathing room to save or maintain their planned economy after electing a liberal party</sup>
  - MIN_NUM_FACTORIES_PER_STATE_BEFORE_DELETING_LASSIEZ_FAIRE: **2 > 9** <sup>Gives the user more breathing room to save or maintain their planned economy after electing a liberal party</sup>
  - FACTORY_UPGRADE_EMPLOYEE_FACTOR: **0.8 -> 0.75** <sup>Convenience change</sup>
  - CAPITALIST_BUILD_FACTORY_STATE_EMPLOYMENT_PERCENT: **0.7 > 1.1** <sup>Changes aimed to prevent Capitalists from creating new factories</sup>
  - NONCORE_TAX_PENALTY: **-0.05 -> -0.10**
  - BASE_COUNTRY_TAX_EFFICIENCY: **0.2 -> 0.22**



- Misc
  - AI Army Changes[^8]
  - AI_CAVALRY_PROPORTION -   **0.15 > 0.1**  :chart_with_downwards_trend:
  - AI_SUPPORT_PROPORTION -   **0.3 -> 0.5**  :chart_with_downwards_trend:
  - AI_SPECIAL_PROPORTION -   **0.15 -> 0**   :chart_with_downwards_trend:
  - REDUCTION_AFTER_DEFEAT -  **3.0 > 4.0**   :chart_with_upwards_trend: <sup>After a rebellion is being defeated in combat, its pop militancy will be divided by this number.</sup>
  - PEACE_BASE_RELUCTANCE -   **20 -> 15**    :chart_with_downwards_trend: <sup>AI base stubbornness to refuse peace.</sup>
  - Disabled Newspapers
  - Disabled Crises


Here is a simple footnote.

A footnote can also have multiple lines[^2].

[^1]: Makes larger navies of low quality less effective against smaller navies of lower quality. Incentivises high tier ships. 
[^2]: Reintroduces randomness to Gas and Gas defense by nerfing its potential output overall. 
  Allows Gas to become an important consideration for Players once again.
[^3]: Makes it so players cannot win wars just off ticking war score, you must also be winning via other factors by atleast 25%.
[^4]: Removes diplo point cost for majority of actions and all player to player interactions, but keeps diplo point cost for actions related to influencing nations
  I.e. increasing relations or decreasing relations
[^5]: Allows large nations like the Ottomans to still be influenced, even when they scale
[^6]: Gives the user more breathing room to save or maintain their planned economy after electing a liberal party
[^7]: Changes aimed to prevent Capitalists from creating new factories
[^8]: Makes the AI build Reno meta stacks, so they are less like paper tigers.





Examples
 
## [Unreleased] - yyyy-mm-dd
 
Here we write upgrading notes for brands. It's a team effort to make them as
straightforward as possible.
 
### Added
- [PROJECTNAME-XXXX](http://tickets.projectname.com/browse/PROJECTNAME-XXXX)
  MINOR Ticket title goes here.
- [PROJECTNAME-YYYY](http://tickets.projectname.com/browse/PROJECTNAME-YYYY)
  PATCH Ticket title goes here.
 
### Changed
 
### Fixed
 
## [1.2.4] - 2017-03-15
  
Here we would have the update steps for 1.2.4 for people to follow.
 
### Added
 
### Changed
  
- [PROJECTNAME-ZZZZ](http://tickets.projectname.com/browse/PROJECTNAME-ZZZZ)
  PATCH Drupal.org is now used for composer.
 
### Fixed
 
- [PROJECTNAME-TTTT](http://tickets.projectname.com/browse/PROJECTNAME-TTTT)
  PATCH Add logic to runsheet teaser delete to delete corresponding
  schedule cards.
 
## [1.2.3] - 2017-03-14
 
### Added
   
### Changed
 
### Fixed
 
- [PROJECTNAME-UUUU](http://tickets.projectname.com/browse/PROJECTNAME-UUUU)
  MINOR Fix module foo tests
- [PROJECTNAME-RRRR](http://tickets.projectname.com/browse/PROJECTNAME-RRRR)
  MAJOR Module foo's timeline uses the browser timezone for date resolution 

Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].

[^1]: My reference.
[^2]: To add line breaks within a footnote, prefix new lines with 2 spaces.
  This is a second line.
