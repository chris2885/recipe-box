2026-11-03

- Anonymous GET /recipes → 200 OK, returns all recipes including non-public ones (e.g. "Secret family hot sauce" with `"is_public": false`).
- Anonymous PATCH /recipes/1 → 200 OK, updates the recipe title to "Totally Hacked Shakshuka" and returns the modified recipe. No identity or permission checked.
- Anonymous DELETE /recipes/1 → 204 NO CONTENT, recipe with id 1 is permanently removed. No identity or permission checked; any caller can delete recipes by ID.
