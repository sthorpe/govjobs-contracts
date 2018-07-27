# GovJobs Contracts

## Government Agencies create digital Identity

### Anyone can create a contract which assigns an agency
   - Agency assigning contracts must contain
      - Agency parent contract (Contract ID: only assigned if this agency’s rules can be changed by another agency)
      - Agency Identity (public key which allows control)
      - Agency rules (how the agency must run)
      - Wallet (funds controlled by the agency Identity and used to enforce the Agency rules)
   - Agency (contracts) can create child agency contracts
      - Same as Agency but have a “parent” field linking to it’s parent agency contract
      - Parent agencies can change their child agency’s rules
   - All agency contracts can create rule contracts
      - Rule contracts must contain
      - Rules that will be enforced
      - Wallet (allocation of funds which have to go towards enforcing this rule)
