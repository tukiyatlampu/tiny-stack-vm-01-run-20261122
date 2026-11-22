# TEST_RESULTS (Node v24.22.1, kit scorer)

- Practice set (kit, 40 inst): **1,000,000** (40/40, passed=1)
- Fresh set A/B (kit generator, new seeds): **1,000,000** each (40/40)
- Fuzz F1/F2/F3 vs reference vm.mjs (120 random + 8 hand edge incl. empty prog, truncated PUSH32, opcode 0xFF): **1,000,000** each
- Determinism (practice, 2 runs): byte-identical
- Worst case (40x infinite loop, 40M steps): 674 ms, 40/40 trap 10 (limit 60 s)
- Practice wall time: ~0.27 s / 40 instances
- grade-local --driver process: 40,000/40,000, score 1,000,000, L1 regrade byte-identical
- Judge SolAPI: NOT RUN — HTTP 503 all day 2026-11-22 (5 attempts); self-critique vs vm.mjs substituted. No judge score claimed.
