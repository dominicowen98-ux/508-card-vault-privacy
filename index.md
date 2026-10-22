# 508 Card Vault Privacy Policy

## Personal store tracker

This private, single-seller application stores sales and expense records on its owner’s computer. It does not sell personal data. OAuth sign-in codes pass through this HTTPS callback and are forwarded to the local app; user access/refresh tokens are stored locally, not in this Worker.

Authenticated eBay deletion notifications are reduced to one-way identifier hashes and queued in Cloudflare D1 until processed locally. Their identifier hashes are removed from the inbox after acknowledgment. The local app deletes matching records, retains a minimal hashed suppression list to prevent re-import, and pauses for owner review when it cannot safely associate older records. Cloudflare and eBay also apply their respective privacy policies.

The operator must monitor deletion handling, remove affected external CSV files/backups, and keep the app running regularly. This is not a shared or commercial service.
