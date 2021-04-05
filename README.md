# hw5
substrate_hw5


* Q1
  * 3 common macros:
    1. decl_storage
    2. decl_module
    3. decl_event

  * 3 common storage data structures:
    1. 单值类型，e.g. Vec, u8,
    2. 简单映射: Map
    3. 双键映射: Double Key Map

* Q2: Compiled against 3.0.0, please copy over directories pallet/poe and runtime to a raw substrate3.0.0 NoteTemplate to compile
  1. Chain running
  ![Compile & chain running](doc/chain_running.png?raw=true)

  2. Claims Initial State
  ![Claims initial state](doc/claims_state00.png?raw=true)

  3. Alice claims 0x00
  ![alice 0x00](doc/alice_claims_0x00.png?raw=true)

  4. Bob claims 0x00 FAILED
  ![bob 0x01](doc/bob_claims_0x00_failed.png?raw=true)

  5. Bob claims 0x01
  ![bob 0x01](doc/bob_claims_0x01.png?raw=true)

  6. submitted 2 claims
  ![2 claims total](doc/claims_ѕtate01.png?raw=true)

  6. Alice cannot revoke Bob's claim
  ![alice failed to revoke bob's claim](doc/alice_revokes_bob_failed.png?raw=true)

  7. Bob revoke own claim successfully
  ![bob revoke own claim successfully](doc/bob_revokes_own_claim.png?raw=true)


* Q3 embedded in pallet/poe.rs/transfer_claim
  1. Claims available 
  ![claims initial state](doc/claims_state01.png?raw=true)

  2. Self-transfer failed
  ![self transfer failed](doc/alice_transfers_self_failed?raw=true)

  3. Transfer something I don't own failed
  ![transfer not mine failed](doc/alice_transfers_0x01_failed?raw=true)

  4. Claim transfer success
  ![claim transfer success](doc/alice_transfers_bob_0x00?raw=true)

  5. Bob (5FHneW46xGXgs5mUiveU4sbTyGBzmstUspZC92UhjJM694ty) owns 2 claims now
  ![claims final state](doc/claims_state02.png?raw=true)

