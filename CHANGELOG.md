
# Change Log
All notable changes to this project will be documented in this file.
 
The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

This file uses the date format of YYYY-MM-DD. 

## [0.1] - UNRELEASED
 
 
### Added
- Added Ethan Leaders
  - Takes the PUIR approach of splitting attack and defense into separate columns, and adding colours to good leaders while retaining Vanilla leader distribution
- Added Peanuts Map Mod and Blue Interface Borders Graphics Packs
- Added custom Navy Units UI


### Changed
**Navy rework**
- Defines
  - NAVAL_BASE_SUPPLY_SCORE_BASE **10 > 2**,
  <br /><sup>Makes supply much scarcer, allowing heavy ships to be significantly buffed</sup>
  - NAVAL_COMBAT_STACKING_TARGET_CHANGE **0.03 -> 0.1** :chart_with_upwards_trend:
  - NAVAL_COMBAT_STACKING_TARGET_SELECT **0.2 -> 0.3** :chart_with_upwards_trend:
  - NAVAL_COMBAT_MAX_TARGETS **6 -> 4** :chart_with_downwards_trend:
  <br /><sup>Makes larger navies of low quality less effective against smaller navies of lower quality. Incentivises high tier ships.</sup>

- Localisation and UI
  - Commerce Raiders are now called Steam Sloops
  - Heavy Ship Text is now coloured in Blue
  - Order of ships has changed, transports are on the left, then it goes in order of Ship Design Tiers with the Light Ship preceding the Heavy Ship
  - Each tier of ship design has been given a unique colour and has been given increased spacing between other tiers to distinguish them

- Tech and invention changes
  - Unlocks
    - Iron Steamers **1836 -> 1840**
    <br /><sup>:warning: **NOTICE** Recommend removing this tech from UK and France in Vanilla based mods and giving the Naval Build Time tech instead</sup>
    - Steel Steamers **1860 -> 1855**
    - Modern Naval Doctrine **1914** -> **1905**
    - Oil Driven Ships **1914** -> **1910**
    - Modern Naval Training **1919** -> **1910**
    - Modern Naval Design **1919** -> **1910**
    - Naval Integration **1919** -> **1910**
  - Heavy ship discovery chance has decreased, but you can take other techs to increase the chance
    - Dreadnought ship discovery chance is very low, but increases dramatically if another country discovers them
  - Ironclads and Monitors are now distinct, Ironclads unlock with Iron Steamers while Monitors unlock with Steel Steamers
  - Monitors have been buffed to be a stronger version of Ironclads, but weaker than Battleships
  - Cruisers has been nerfed to be the light ship equiavlent of Monitors
  - Torpedo attack has been made scarce. Steam Sloops can get a maximum of 1 and Cruisers can get a maximum of 8 in 1914 (4 beforehand, 1 initially)
  - Evasion has been generally nerfed, light ships have 10% evasion generally, with Cruisers having 15%
    - Very small evasion has been added to transports
  - Monitors can now not be built overseas (seems like an oversight from Vanilla?)
  
- Mechanics
  - Heavy ships are now the strongest ships on the sea
  - Heavy ships are the **ONLY** ships which cost naval capacity. Scaling by 1 additional cost per tier of ship
    - A level 6 naval base will allow you to build 2 dreadnoughts.
  - Light ships are weaker than heavy ships, but cost no supply.
  - Light ships will receive occasional invention buffs to help them keep up with heavies.
  - Supply Costs, Maintenance Costs, Stats, Speed and Colonial Points have all been adjusted.


**War**
  - TWS_CB_LIMIT_DEFAULT **100 -> 75** :chart_with_downwards_trend:
  <br /><sup>Makes it so players cannot win wars just from ticking war score, you must also be winning via other factors by atleast 25%.</sup>
  - MOBILIZATION_SPEED_RAILS_MULT **3.0 -> 3.5** :chart_with_upwards_trend: 
  <br /><sup>Small buff to high tech nations / Railroads</sup>
  - Gas changes
    - Defines GAS_ATTACK_MODIFIER **3 -> 1**
    <br /><sup>Reintroduces randomness to Gas and Gas defense by nerfing its overall impact, allowing Gas to be relevant again.</sup>
    - Invention
      - Gas Attack discover chance if at war **0 -> 5%** :new:
      - Gas Defense discover chance if at war with someone with gas attack **5 -> 11%** :chart_with_upwards_trend:
  - Forts activate at Strategic Mobility instead of Post Napoleonic Thought
  - Infiltration does not award a fort level
  - Mobilization *Economy* Impact added to Jingoism idea 0 -> 25% :new:
  - Mobilization Impact from Jingoism reduced from **400% -> 20%** :chart_with_downwards_trend:
  - Mobilization Impact from Pro Military reduced from **300% -> 10%**  :chart_with_downwards_trend:
  - Mobilization Impact removed from Anti Military and Pacifism :x:
  - Mobilization Impact added to Equality National value of **75%** :new:
  - Mobilization Impact added to Order National value of **100%** :new:
  - Mobilization Impact added to Liberty National value of **200%** :new:
  - Mobilization *Economy* Impact increased for Liberty National value **0.75 -> 2.25** :chart_with_upwards_trend:
  - Added Mobilization Impact increases to the Light Armament line of tech :new:
  - War Reps total years reduced from **5 -> 2** :chart_with_downwards_trend:
  - Max Warscore from Battles reduced from **50 --> 25** :chart_with_downwards_trend:
  - Releasing nations reduces infamy by **5 -> 2** :chart_with_downwards_trend:


**Diplomacy**
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
  - BASE_MONTHLY_DIPLOPOINTS **0.3 -> 0.5** :chart_with_upwards_trend:
  <br /><sup>Removes diplo point cost for majority of actions and all player to player interactions, but keeps diplo point cost for actions related to influencing nation s</sup>
- MAKE_CB_RELATION_LIMIT **100 -> 120** :chart_with_upwards_trend:
- LARGE_POPULATION_INFLUENCE_PENALTY **-0.4 -> -0.25** :chart_with_downwards_trend:
  <br /><sup>Allows large nations like the Ottomans to still be influenced, even when they scale</sup>
- War Subsidies percent of imports paid for increased from **0.25 -> 0.33** :chart_with_upwards_trend:


**Economy**
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
  - Forts
    - Max level **6 -> 4** :chart_with_downwards_trend: 
    - Good cost increased
      - Artillery **40 -> 333** :chart_with_upwards_trend: 
      - Small Arms **50 -> 333** :chart_with_upwards_trend: 
      - Canned Food **0 -> 333** :new:
  - Naval Base
    - Goods cost increased
      - Cement **100 -> 200** :chart_with_upwards_trend: 
      - Steel **100 -> 333** :chart_with_upwards_trend: 
      - Artillery **0 -> 200** :new:
  - Railroad
    - Goods cost increased
      - Timber **100 -> 200** :chart_with_upwards_trend: 
      - Steel **100 -> 200** :chart_with_upwards_trend: 
  - Machine Parts Factory
    - Goods cost adjusted
      - Iron **200 -> 350** :chart_with_upwards_trend:
      - Cement **200 -> 350** :chart_with_upwards_trend: 
      - Machine Parts **200 -> 0** :x:
  - Steel Factory
    - Goods cost reduced
      - Machine Parts - Iron **200 -> 100** :chart_with_downwards_trend:
  - Laissez Faire factory output bonus **0.05 -> 0.075** :chart_with_upwards_trend:
  - Interventionism factory output bonus **0 -> 0.025** :new:
  - Planned economy factory throughput bonus **0.05 -> 0.075** :chart_with_upwards_trend:
    

**Misc**
  - AI Army Changes
  - AI_CAVALRY_PROPORTION -   **0.15 > 0.1**  :chart_with_downwards_trend:
  - AI_SUPPORT_PROPORTION -   **0.3 -> 0.5**  :chart_with_downwards_trend:
  - AI_SPECIAL_PROPORTION -   **0.15 -> 0**   :chart_with_downwards_trend:
  <br /><sup>Makes the AI build Reno meta stacks, so they are less like paper tigers. Although it is likely these defines don't function.</sup>
  - REDUCTION_AFTER_DEFEAT -  **3.0 > 4.0**   :chart_with_upwards_trend: 
  <br /><sup>After a rebellion is being defeated in combat, its pop militancy will be divided by this number. Increased to give players more breathing room between rebellions.</sup>
  - PEACE_BASE_RELUCTANCE -   **20 -> 15**    :chart_with_downwards_trend: 
  <br /><sup>AI base stubbornness to refuse peace. Decreased to make dealing with AI slightly less difficult.</sup>
  - Pacifism now gives **-0.05** infamy monthly :new:
  - Pacifism now gives **-10% Unit Attack** :new:


### Removed
  - Disabled Newspapers :x:
  - Disabled Crises :x:
  - Disabled pops from building new factories or opening closed factories via economic policy rules :x: