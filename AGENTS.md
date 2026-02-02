# AGENTS.md — OpenClaw Inspector

## Development Rules

### Testing
- After every change, run `npm test` to make sure all existing tests pass.
- Every new feature or bug fix must have test coverage before merging.
- Run `npx cypress run` for E2E tests when UI behavior changes.

### Build
- Run `npx vite build` after changes — must compile without errors.
- Restart `node server.js` after build to serve updated dist.

### Workflow
1. Make changes
2. `npm test` — all tests pass
3. `npx vite build` — clean build
4. Manual verification on `http://localhost:9100`
5. `git commit` + `git push`
6. Update beads: `bd close` / `bd sync`
