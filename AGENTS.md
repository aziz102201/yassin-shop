# Yassin Shop project conventions

- Keep business-specific content in `artifacts/yassin-shop/src/data/shop-config.ts`; do not scatter product or contact facts through page components.
- Never invent products, prices, variants, stock, policies, delivery promises, payment methods, or contact details. Empty configuration should produce a useful, honest UI state.
- Keep the storefront French-first, mobile-first, and accessible. Use Wouter for routes and lucide-react for interface icons.
- Add stable `data-testid` attributes to interactive controls and important dynamic content.
- Run `pnpm --filter @workspace/yassin-shop run typecheck` after frontend changes. The artifact workflow supplies `PORT` and `BASE_PATH` for local preview.