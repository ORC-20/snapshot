# ORC-20 Nirvana Upgrade Snapshot

This snapshot file serves as the genesis file for the ORC-20 Nirvana upgrade, guiding the continued operation based on the snapshot data. The snapshot is created with the following rules:

1. **Snapshot Block Height**: The block height of the snapshot is 818,418.

2. **Data Source**: The snapshot data is sourced from https://geniidata.com/ordinals/index/orc20.

3. **Data Preservation**: The snapshot includes token information and user balance states, excluding transaction records. Indexers can still import previous data for user display.

4. **Token Validity**: A token is considered invalid and excluded from the snapshot if its parameters do not meet the new protocol requirements (e.g., max value exceeding `max(uint_64)`) and the token's holder count is 0. Both conditions must be met.

5. **Transaction Validity**: Transactions not executed at block height 818,418 are invalid.
