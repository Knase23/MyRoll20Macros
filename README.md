# Knase Roll20 Macros
#### Clarifications:
  - Normal: 1d20
  - Advantage: 2d20 take the higher of the two.
  - Disadvantage: 2d20 take the lower of the two.

## Useful Macro code for dnd5e on Roll20
  Available always:
  - **#Roll20+Mod** - See "Macro code for rolling D20 and add modifier"

Available when having a token selected
  - **#RollForInitiative** - See "Macro code for rolling Initiative"

### Macro code for rolling Initiative.
  > /r ?{Roll Initiative|Normal ,1d20  | Advantage , 2d20kh1  | Disadvantage , 2d20kl1}  + @{selected|initiative_bonus} &{tracker} Roll for Initiative  

  It will give you a menu to select Advantage, Normal or Disadvantage. And then uses the selected tokens attribute for Initiative. And then add it to Roll20s Turn Tracker.  
  **Note:** You need to have a character sheet or a attribute named *initiative_bonus* attached to your **selected token**  
  If you want to type it in yourself use this one:
  > /r ?{Roll Initiative|Normal ,1d20  | Advantage , 2d20kh1  | Disadvantage , 2d20kl1}  + ?{Initiative Modifier|0} &{tracker} Roll for Initiative

### Macro code for rolling D20 and add modifier
  > /r ?{Roll Initiative|Normal ,1d20  | Advantage , 2d20kh1  | Disadvantage , 2d20kl1} + ?{Modifier|0}

  It will give you a menu for rolling with Advantage, Disadvantage or Normal. Then you can add your modifier in the next menu. If you have a negative modifier just write a negative number in the appropriate area.
