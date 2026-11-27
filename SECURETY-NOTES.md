# Security baseline

2026-11-26

- Anonymous GET /recipes → 200 OK, returns all recipes including `"Secret family hot sauce"` where `is_public: false`.
- Anonymous DELETE /recipes/2 → succeeds; follow-up GET /recipes/2 returns `{"error": "recipe not found"}`.
