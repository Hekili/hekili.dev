---
layout: default
title: Hekili - Action Lists
section: Action Lists
datatable: true
theme: jekyll-pages-midnight
datatable: true
---

Priorities are comprised of Action Lists, which are made up of Actions and their conditions.  This model is based on SimulationCraft, where a character profile will have two or more action lists.  The built-in action lists are `precombat` -- for actions before combat begins -- and the unnamed default once combat starts.

 Additional action lists can be created and tested from the default action list as well as from each other using `run_action_list` and `call_action_list`.  `run_action_list` will cause the addon to exit its current action list and test the named acdtion list it selected.  `call_action_list` is similar, but will return to the calling action list afterward, if a recommendation has not yet been found.

 SimulationCraft | Hekili
 ----------------|-------
 SimulationCraft will attempt to execute each line of the `precombat` action list once before the start of simulated combat. | Hekili will test the entries in the `precombat` action list outside of combat, but may also recommend `essential` abilities during combat.<br /><br />Essential abilities are usually things like maintenance buffs or summoning pets.
