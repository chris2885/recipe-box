2026-11-03

- Anonymous GET /recipes → 200 OK, returns all recipes including non-public ones (e.g. "Secret family hot sauce" with `"is_public": false`).
- Anonymous PATCH /recipes/1 → 200 OK, updates the recipe title to "Totally Hacked Shakshuka" and returns the modified recipe. No identity or permission checked.
