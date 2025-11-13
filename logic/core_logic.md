# Core Logic — Scratch Battle Royale

## 1. Player Movement
- WASD or arrow keys move the player.
- Player uses “change x by” and “change y by” blocks.
- Movement includes collision checks with obstacles.

## 2. Shooting System
- Bullet is a clone of a sprite.
- When player presses shoot button:
  - Create clone of Bullet
  - Point clone toward mouse or enemy
  - Move clone using “repeat until” or “move 10 steps”
  - If clone touches enemy: reduce enemy HP

## 3. Enemy AI
- Each enemy continuously:
  - Points toward player
  - Moves forward slowly
  - Avoids obstacles using bounce logic
  - Deals touch damage to player

## 4. Safe Zone Shrinking
- Safe zone is a large circle sprite.
- Every few seconds, reduce its size by a small factor.
- If player is outside safe zone → take damage over time.

## 5. Health & Damage
- Player and enemies each have HP variables.
- Collisions or bullets reduce HP.
- When HP ≤ 0 → sprite “dies.”

## 6. Win / Lose Conditions
- If all enemies’ HP reach 0 → Victory screen.
- If player’s HP reaches 0 → Game Over screen.
