# Code Review Checklist

## Correctness
- Clear inputs/outputs, edge cases handled
- Idempotency where required (payments, webhooks, retries)
- Error handling is explicit and consistent

## Security
- Authorization enforced server-side
- Input validation for all external inputs
- Secrets never logged
- Safe defaults, least privilege
- Rate limiting applied on sensitive actions

## Performance
- Avoid N+1 patterns
- Cache boundaries are clear
- DB indexes considered for critical queries
- Payload sizes controlled

## Maintainability
- Naming and structure are consistent
- Tests cover critical paths
- Logging is structured and actionable
