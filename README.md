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

  2. Alice submit claim 0x00
  ![alice 0x00](doc/alice_claims_0x00.png?raw=true)

  2. Bob cannot claim 0x00
  ![bob 0x01](doc/bob_claims_0x00_failed.png?raw=true)

  4. Bob submit claim 0x01
  ![bob 0x01](doc/bob_claims_0x01.png?raw=true)

  5. submitted 2 claims
  ![2 claims](doc/claims_ѕtate01.png?raw=true)

  6. Alice cannot revoke Bob's claim
  ![alice failed to revoke bob's claim](doc/alice_revoke_bob_failed.png?raw=true)

  7. Bob revoke own claim successfully
  ![bob revoke own claim successfully](doc/bob_revoke_own_claim_success.png?raw=true)


* Q3 embedded in Q2 pallet/poe.rs
  1. Claims available 
  ![claims available](doc/claims_available.png?raw=true)

  2. Claim transfer failed
  ![claim transfer failed](doc/claim_transer_failed?raw=true)

  3. Claim transfer success
  ![claim transfer success](doc/claim_transer_success?raw=true)
