# LogLine Projection Kernel Contracts

These contracts are the machine boundary for the Projection Kernel Pack. They validate object shape, boundary, doubt, activation, policy, receipts, custody, revocation, and conformance without exposing private kernel algorithms.

Editorial rule: a contract exists to prevent plausible language from crossing a boundary without shape, proof, state, and receipt.

## Families

### core

- `core/act.schema.json`
- `core/act-envelope.schema.json`
- `core/act-hash.schema.json`
- `core/act-admission-request.schema.json`
- `core/act-admission-result.schema.json`
- `core/ledger-entry.schema.json`
- `core/ledger-page.schema.json`
- `core/aux.schema.json`
- `core/jcs-canonicalization.profile.json`

### boundaries

- `boundaries/source-boundary.schema.json`
- `boundaries/evidence-boundary.schema.json`
- `boundaries/projection-boundary.schema.json`
- `boundaries/rights-boundary.schema.json`
- `boundaries/policy-boundary.schema.json`
- `boundaries/custody-boundary.schema.json`
- `boundaries/agent-boundary.schema.json`
- `boundaries/external-effect-boundary.schema.json`

### projections

- `projections/projection-request.schema.json`
- `projections/projection.schema.json`
- `projections/projection-summary.schema.json`
- `projections/projection-inspection.schema.json`
- `projections/projection-lineage.schema.json`
- `projections/projection-cache-entry.schema.json`
- `projections/projection-build-result.schema.json`
- `projections/projection-replay-request.schema.json`
- `projections/projection-replay-result.schema.json`
- `projections/projection-diff.schema.json`
- `projections/projection-expiry.schema.json`

### lenses

- `lenses/lens.schema.json`
- `lenses/lens-id.schema.json`
- `lenses/lens-registry.schema.json`
- `lenses/lens-version.schema.json`
- `lenses/lens-input-contract.schema.json`
- `lenses/lens-output-contract.schema.json`
- `lenses/lens-selection-trace.schema.json`
- `lenses/lens-redaction-policy.schema.json`

### doubt

- `doubt/doubt-state.schema.json`
- `doubt/doubt-map.schema.json`
- `doubt/doubt-claim.schema.json`
- `doubt/doubt-summary.schema.json`
- `doubt/doubt-transition.schema.json`
- `doubt/doubt-blocker.schema.json`
- `doubt/uncertainty-preservation.schema.json`
- `doubt/contested-claim.schema.json`
- `doubt/stale-claim.schema.json`
- `doubt/human-required.schema.json`

### activation

- `activation/activation-state.schema.json`
- `activation/activation-map.schema.json`
- `activation/activation-request.schema.json`
- `activation/activation-result.schema.json`
- `activation/activation-transition.schema.json`
- `activation/activation-blocker.schema.json`
- `activation/activation-permission.schema.json`
- `activation/activation-readiness.schema.json`
- `activation/safe-next-action.schema.json`

### evidence

- `evidence/evidence-item.schema.json`
- `evidence/evidence-pointer.schema.json`
- `evidence/evidence-claim.schema.json`
- `evidence/evidence-set.schema.json`
- `evidence/evidence-gap.schema.json`
- `evidence/evidence-check.schema.json`
- `evidence/evidence-chain.schema.json`
- `evidence/evidence-redaction.schema.json`
- `evidence/evidence-retention.schema.json`

### policies

- `policies/policy.schema.json`
- `policies/policy-set.schema.json`
- `policies/policy-decision.schema.json`
- `policies/policy-blocker.schema.json`
- `policies/policy-conflict.schema.json`
- `policies/policy-exception.schema.json`
- `policies/policy-version.schema.json`
- `policies/policy-scope.schema.json`
- `policies/policy-required-human.schema.json`

### scorecards

- `scorecards/scorecard.schema.json`
- `scorecards/scorecard-public.schema.json`
- `scorecards/projection-scorecard.schema.json`
- `scorecards/sealability-scorecard.schema.json`
- `scorecards/anchor-scorecard.schema.json`
- `scorecards/evidence-scorecard.schema.json`
- `scorecards/policy-scorecard.schema.json`
- `scorecards/trust-scorecard.schema.json`
- `scorecards/score-explanation.schema.json`

### diamonds

- `diamonds/diamond-candidate.schema.json`
- `diamonds/diamond.manifest.schema.json`
- `diamonds/diamond.manifest.public.schema.json`
- `diamonds/diamond-seal-request.schema.json`
- `diamonds/diamond-seal-result.schema.json`
- `diamonds/diamond-verification.schema.json`
- `diamonds/diamond-lineage.schema.json`
- `diamonds/diamond-custody.schema.json`
- `diamonds/diamond-rights.schema.json`
- `diamonds/diamond-license.schema.json`
- `diamonds/diamond-constraint.schema.json`
- `diamonds/diamond-revocation.schema.json`
- `diamonds/diamond-expiry.schema.json`
- `diamonds/diamond-supersession.schema.json`
- `diamonds/diamond-redemption.schema.json`

### anchors

- `anchors/anchor-request.schema.json`
- `anchors/anchor-result.schema.json`
- `anchors/anchor-candidate.schema.json`
- `anchors/anchor-boundary.schema.json`
- `anchors/anchor-permission.schema.json`
- `anchors/anchor-failure.schema.json`
- `anchors/no-safe-anchor.schema.json`
- `anchors/agent-anchor-context.schema.json`
- `anchors/agent-lost-state.schema.json`

### agents

- `agents/agent-identity.schema.json`
- `agents/agent-session.schema.json`
- `agents/agent-purpose.schema.json`
- `agents/agent-permission.schema.json`
- `agents/agent-grounding-report.schema.json`
- `agents/agent-memory-read.schema.json`
- `agents/agent-memory-write-request.schema.json`
- `agents/agent-action-proposal.schema.json`
- `agents/agent-response-contract.schema.json`

### effects

- `effects/effect-spec.schema.json`
- `effects/effect-intent.schema.json`
- `effects/effect-readiness.schema.json`
- `effects/effect-airlock-request.schema.json`
- `effects/effect-commit-result.schema.json`
- `effects/effect-failure.schema.json`
- `effects/effect-compensator.schema.json`
- `effects/effect-idempotency.schema.json`
- `effects/external-call.schema.json`
- `effects/irreversible-effect.schema.json`
- `effects/notification-effect.schema.json`

### receipts

- `receipts/receipt.schema.json`
- `receipts/receipt-chain.schema.json`
- `receipts/admission-receipt.schema.json`
- `receipts/projection-receipt.schema.json`
- `receipts/activation-receipt.schema.json`
- `receipts/anchor-receipt.schema.json`
- `receipts/seal-receipt.schema.json`
- `receipts/redeem-receipt.schema.json`
- `receipts/revoke-receipt.schema.json`
- `receipts/effect-receipt.schema.json`
- `receipts/audit-receipt.schema.json`

### vault

- `vault/vault-entry.schema.json`
- `vault/vault-pointer.schema.json`
- `vault/vault-receipt.schema.json`
- `vault/vault-custody-event.schema.json`
- `vault/vault-access-grant.schema.json`
- `vault/vault-access-denial.schema.json`
- `vault/vault-retention-policy.schema.json`
- `vault/vault-export-manifest.schema.json`

### api

- `api/error.schema.json`
- `api/pagination.schema.json`
- `api/auth-context.schema.json`
- `api/request-context.schema.json`
- `api/response-envelope.schema.json`
- `api/webhook-event.schema.json`
- `api/api-receipt-envelope.schema.json`
- `api/idempotency-key.schema.json`

### cli

- `cli/command-result.schema.json`
- `cli/command-context.schema.json`
- `cli/command-receipt.schema.json`
- `cli/command-error.schema.json`
- `cli/command-dry-run.schema.json`

### conformance

- `conformance/vector.schema.json`
- `conformance/vector-suite.schema.json`
- `conformance/vector-result.schema.json`
- `conformance/conformance-report.schema.json`
- `conformance/compatibility-claim.schema.json`
- `conformance/implementation-profile.schema.json`
- `conformance/failure-case.schema.json`

### packaging

- `packaging/pack.manifest.schema.json`
- `packaging/pack-index.schema.json`
- `packaging/pack-node.schema.json`
- `packaging/pack-activation-order.schema.json`
- `packaging/pack-invariant.schema.json`
- `packaging/pack-release.schema.json`
- `packaging/pack-signature.schema.json`
- `packaging/pack-license.schema.json`
