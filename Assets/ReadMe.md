# Plan

## 17th Feb

### Install the system of update Stamina

- To prepare the script of UpdateStamina.cs
  - Input: float amount, bool isDamage
  - Output: N/A
  - Work: to update the CurrentStamina and MaxStamina of Stamina UI depends on the argument's number
    - details: if the isDamage is true, Decrease the CurrentStamina and MaxStamina, then refresh UI
    - details: if the isDamage is false, Decrease the CurrentStamina only, then refresh UI

#### When it comes to use: Move

- For making this function, you implement this system into the CharacterController.cs and invoke UpdateStamina
  - The arguments depends on the amount of MovingSpeed for UpdateStamina
    - if the alternativeInput.magunitude were over 0.7 \* root2, the amount is gonna be -0.5f[%]
    - if the alternativeInput.magunitude were over 0.7 \* root2, the amount is gonna be -0.8f[%]

#### When it comes to use: Avoid

- For making this function, you implement this system into the CharacterController.cs and invoke UpdateStamina
  - The arguments depends on the amount is gonna be -25.0f[%]

#### When it comes to use: Jump

- For making this function, you implement this system into the CharacterController.cs and invoke UpdateStamina
  - The arguments depends on the amount is gonna be -2.0f[%]

#### When it comes to use: Attack1 & Attack2

- For making this function, you implement this system into the CharacterController.cs and invoke UpdateStamina
  - The arguments depends on the amount is gonna be -20.0f[%]

#### When it comes to use: Idle or Walk

- For making this function, you implement this system into the CharacterController.cs and invoke UpdateStamina
  - The arguments depends on the amount is gonna be 1.0f[%]

## 18th Feb 21th Wed

### DamageCalcuration

- if character and monster are damaged which means depends on the current stamina , chagen how easy to blow away
  - need monster stamina script
- if character or monster are damaged, change the max stamina and lock the max stamina in intended seconds
- if character blow away so far from the damage point, the character destroy and update the trust lv

## 23 Feb

- I'd like to turn on the Lock on system automatically when enemy enter the player teritory, if the enemy out of the teritory, the system are made turn off as well.
  - if the Lock on system turning on, lock on camera should chase the colsest enemy from player
    - Emit ray from player to 60m

## 24 Feb

- if you beated enemy, change trust lv
- if you are beated by enemy, trust lv gowing down
