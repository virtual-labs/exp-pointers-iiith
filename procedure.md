This simulation has two modules:

1. Call By Value
2. Call By Reference

Open the simulation page and click the thumbnail of the module you want to run.

#### Steps for Call By Value

1. Click **Start** to begin execution.
2. Observe the first highlighted code line in the Program Code panel.
3. Click **Next** to move to the next execution step.
4. At each step, observe all three panels together:
   - **Program Code**: currently executing line is highlighted.
   - **Memory Map**: addresses and stored byte values are updated.
   - **Code Output / Explanation**: printed output and reasoning for that step.
5. Continue clicking **Next** to trace declaration of `A`, declaration of pointer `P`, assignment `P = &A`, dereferencing `*P`, and update of `A` through pointer.
6. Use **Back** to revisit previous steps and verify how values and addresses change in reverse order.
7. Continue until program execution completes; the simulation resets to initial state for a fresh run.

#### Steps for Call By Reference

1. Click **Start** to begin execution.
2. Click **Next** to step through `main()` and the function call to `swap(&A, &B)`.
3. Observe pointer variables in the swap function (`Pa`, `Pb`) and the temporary variable (`temp`) in the **Memory Map**.
4. Track how dereferencing updates original values:
   - `temp = *Pa`
   - `*Pa = *Pb`
   - `*Pb = temp`
5. Compare **Code Output** before and after swap to confirm that values of `A` and `B` are exchanged in caller memory.
6. Use **Back** to inspect reverse flow and confirm each intermediate memory state.
7. Run till completion to see final swapped values and automatic reset.

#### What to Verify During Simulation

1. Every variable occupies a memory address.
2. A pointer stores an address, and dereferencing accesses/modifies value at that address.
3. Passing addresses to a function allows modification of original variables (call by reference behavior).

**Note for Mobile Users:**

This simulation is optimized for desktop computers with larger screens and mouse interaction. If you access this experiment on a mobile device, please rotate your device to **landscape mode** for the best experience. Some features may be limited or harder to use on small screens.
